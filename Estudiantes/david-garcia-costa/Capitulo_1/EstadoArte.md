# Estado del Arte

El capítulo Marco teórico engloba una revisión del estado de la cuestión sobre el tema estudiado en el TFG y que sirve, a su vez, para fundamentar el trabajo.

Para ello, se podrá realizar mediante consulta en bases de datos especializadas, contraste de información, análisis histórico del tema, etc.

## Contexto empresarial de CIC Consulting Informático

CIC Consulting Informático es una empresa de ingeniería y desarrollo de proyectos de informática y comunicaciones (CIC Consulting Informático, s. f.).

En el proceso actual de QA en CIC, el trabajo comienza con una reunión por parte del cliente con el Project Manager, en esa reunión se recogen los requisitos del producto y los casos de uso que debería tener; esto se plasma sobre documentación, en este caso utilizan DRF (Documentos Requisitos Funcionales) y DDS (Documento Diseño Sistema).

A partir de esta información, el ingeniero de QA define casos de prueba que actualmente están en un Excel y algunos de ellos se referencian en una carpeta dentro de VSCode con estructuras Gherkin propio de Kiwi TCMS, pero no se usa ninguna API, ejecuta las pruebas end-to-end en Cypress y documenta incidencias o resultados en las herramientas correspondientes.

Este flujo de trabajo se apoya en herramientas ya existentes detalladas en la foto que se presenta a continuación y en la experiencia del personal de QA, pero mantiene una importante dependencia del análisis manual y de la intervención directa del ingeniero.

![Flujo actual del proceso QA en CIC](fotos/FlujoQA_Actual.svg)

Figura 1. Flujo actual del proceso QA en CIC.

Esto supone una carga significativa para el ingeniero de QA a la hora de interpretar correctamente la documentación de entrada y traducirla a elementos útiles para validar el producto.

A partir del contexto descrito, se pretende mejorar el proceso de QA en CIC Consulting Informático mediante una solución capaz de asistir el análisis de documentación, estructurar requisitos y casos de uso, y transformarlos en casos de prueba útiles para la gestión del testing.

No se trata simplemente de automatizar pruebas en sentido amplio, sino de intervenir en una fase previa del flujo, actualmente con mucho esfuerzo manual.

En consecuencia, el trabajo se centra en estudiar cómo una arquitectura basada en analizar documentos DRF y DDS, extraer información funcional relevante (requisitos funcionales y casos de uso), transformarlo a escenarios Gherkin (Given, When, Then, And) y registrar los casos de prueba en Kiwi TCMS a través de su API y haciendo llamadas en la parte automática con agentes de una API de OpenAI.

## Solución Existente Aproximada

### Quorvex AI

En el testing asistido por Inteligencia Artificial, han comenzado a aparecer soluciones que no se limitan a ejecutar pruebas automatizadas, también intervienen en su construcción a partir de descripciones funcionales en lenguaje natural. Una de las propuestas más próximas al enfoque de este trabajo es Quorvex AI, es una herramienta orientada a la generación automática de tests a partir de especificaciones redactadas en lenguaje natural (NihadMemmedli, s. f.).

El interés de esta solución reside en que plantea un modelo de trabajo en el que la IA no actúa solo como generador de texto, sino como un componente capaz de participar en varias fases del proceso de testing. Al empezar con la especificación inicial, el sistema analiza la información proporcionada, genera un plan de ejecución, construye la prueba correspondiente y por último lo valida sobre la aplicación real. Si detecta errores durante la ejecución, la propia herramienta puede corregir automáticamente parte del código generado con una función de autorreparación (NihadMemmedli, s. f.).

![Diagrama de una solución existente](fotos/quorvex.png)

Figura 2. Diagrama de una solución existente

Nota: Tomado del Github de Quorvex.

Quorvex AI se apoya principalmente en Playwright como framework de automatización y en modelos de lenguaje para interpretar la especificación y la transforma en código ejecutable. Esto le permite convertir descripciones escritas en lenguaje natural en pruebas end-to-end para que las ejecute, esto reduce parte del esfuerzo manual que normalmente requiere la construcción inicial de los tests (NihadMemmedli, s. f.).

Pero, por otra parte, esta solución presenta limitaciones. En primer lugar, el enfoque está claramente orientado a la generación de tests en Playwright, lo que implica una dependencia fuerte de este framework. Y aunque automatiza la construcción de pruebas y contribuye a su reparación, no está tan enfocada en la gestión documental previa ni en la integración con herramientas de gestión de pruebas como Kiwi TCMS, aspectos que sí tienen un peso importante en la propuesta desarrollada en este trabajo.

Por tanto, Quorvex AI puede considerarse como una solución existente y relevante, especialmente por su capacidad para transformar especificaciones naturales en artefactos de testing automatizado. Pero su objetivo se sitúa en una fase distinta del proceso. Mientras Quorvex AI se orienta a la generación directa de tests end-to-end ejecutables, la propuesta de este TFG se centra en una etapa previa, aunque de cierta manera y en líneas futuras se asemeja.

---

[← Volver al Índice](../README.md)
