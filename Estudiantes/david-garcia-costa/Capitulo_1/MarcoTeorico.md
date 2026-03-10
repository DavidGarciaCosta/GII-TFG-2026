La automatización del testing se da como respuesta a la necesidad de ejecutar validaciones de forma repetible, rápida y consistente, mediante el uso de scripts, herramientas y pipelines que permiten reducir parte de la intervención manual y aportar mayor estabilidad en comprobaciones. 

No obstante, la automatización tradicional no siempre resuelve los problemas previos al momento de ejecución. En muchos casos, sigue siendo necesario interpretar requisitos, diseñar escenarios y mantener estructuras de prueba, lo que deja una parte relevante del esfuerzo fuera del alcance de la automatización clásica.  

La aplicación de Inteligencia Artificial al testing supone una evolución respecto a la automatización tradicional. La IA no solo puede ejecutar o asistir tareas repetitivas, sino también participar en procesos de análisis, estructuración y generación de contenido útil para QA, como escenarios de prueba o interpretaciones semánticas de documentación. 

Este cambio de enfoque resulta especialmente interesante cuando la carga del proceso recae sobre tareas cognitivas y documentales. En ese tipo de contexto, la IA puede aportar apoyo no tanto en la ejecución, sino en la fase de preparación del conocimiento para el testing.  
El AI-driven testing hace referencia a enfoques en los que modelos de IA intervienen en la generación, priorización, análisis o mantenimiento de pruebas. A diferencia de las aproximaciones tradicionales, aquí la IA participa en tareas que requieren cierto grado de interpretación y adaptación.  

Una de las aplicaciones más relevantes de la IA en testing es la generación automática o asistida de casos de prueba a partir de requisitos, historias de usuario o documentación funcional. Esta capacidad permite reducir parte del esfuerzo manual y aumentar la velocidad con la que se construyen escenarios iniciales de validación.  

Sin embargo, la calidad del resultado depende de cómo se interprete la entrada, de la consistencia del modelo empleado y del grado de control que se mantenga sobre la transformación. Por ello, la generación automática no debe entenderse como un proceso completamente trivial o garantizado, sino como una línea de apoyo que requiere diseño y validación.  

## Los agentes de IA

Estos representan una evolución respecto al uso de modelos generativos.  
Un agente no solo produce una respuesta de texto, sino que percibe la información, toma decisiones, utiliza herramientas y ejecuta acciones que están orientadas a un objetivo concreto.  
Esto hace que los agentes sean perfectos para procesos con varias etapas conectadas entre sí. En este trabajo, el análisis de documentación, la transformación a Gherkin y la integración con una API son tareas que encajan muy bien en una arquitectura de este tipo.  

## Definición de agente

Un agente puede definirse como una entidad software que percibe información de su entorno, la procesa, toma decisiones y ejecuta acciones en función de un objetivo.  
En términos prácticos, un agente puede combinar un modelo de lenguaje con instrucciones, herramientas, memoria y mecanismos de control, lo que le permite abordar tareas más complejas que una simple generación de texto.  

## Capacidades de percepción, decisión y acción

Las capacidades fundamentales de un agente pueden resumirse en percibir, decidir y actuar. Percibir implica recoger información relevante del entorno o de los datos de entrada. Decidir supone interpretarla y seleccionar una estrategia adecuada. Actuar significa ejecutar una operación útil sobre una herramienta, un sistema o un flujo de trabajo.  
Estas capacidades son especialmente valiosas cuando se desea automatizar procesos encadenados. En este caso, por ejemplo, permiten pasar de un documento de entrada a una salida estructurada y utilizable dentro de una herramienta de gestión de pruebas.  

## Diferencia entre IA generativa e IA agentica

La IA generativa tradicional responde a una entrada mediante la producción de una salida, normalmente textual.  
La IA agentica digamos que incorpora objetivos, uso de herramientas, pasos intermedios y la capacidad de verificación o control del flujo. Por ello, esta última resulta más adecuada para procesos donde se necesita algo más que una respuesta aislada.  
Esta distinción es relevante porque la propuesta del TFG no se limita a pedir al modelo que por ejemplo “redacte” escenarios, sino que requiere una arquitectura capaz de procesar los documentos, estructurar esa información, transformarla y registrarla en una herramienta externa.  
Una característica clave de los agentes es su capacidad para utilizar herramientas externas, como APIs, sistemas de almacenamiento, navegadores o conectores.  
En la propuesta de este TFG, esta capacidad es clave, ya que la integración con Kiwi TCMS mediante API constituye una parte central del flujo. Sin uso de herramientas, la solución quedaría limitada a una simple generación documental sin conexión operativa.  
Por otra parte, para operar de forma coherente, un agente necesita gestionar el contexto, el estado del proceso y, en ciertos casos, mecanismos de memoria. Esto le permite mantener consistencia entre etapas, recordar información relevante y actuar de forma alineada con el objetivo definido.  
En sistemas donde varias tareas se enlazan entre sí, esta gestión resulta especialmente importante. Analizar un documento, estructurar requisitos y convertirlos en escenarios exige conservar relación entre la información original y la salida generada.  

## Sistemas multiagente

Cuando un único agente no es suficiente para abordar todas las tareas necesarias, puede recurrirse a un sistema multiagente.  
Es decir, varios agentes que están programados para realizar tareas concretas colaboran entre sí para resolver un problema común, repartiéndose funciones y manteniendo una coordinación explícita.  
Un sistema multiagente puede definirse como una arquitectura compuesta por varios agentes que colaboran, se coordinan y comparten información para resolver un problema.  

## Coordinación entre agentes

En cuanto a la coordinación no basta con tener varios componentes especializados; se necesita establecer cómo se comunican, en qué orden actúan, qué información comparten y cómo se asegura la coherencia del proceso.  
En la práctica, esta coordinación puede realizarse con un componente orquestador o con reglas de flujo definidas.  

## Especialización de roles

Es una gran ventaja, ya que puede existir un agente centrado en analizar documentos, otro en estructurar requisitos, otro en transformar la información a Gherkin y otro en integrarla con una API externa a través de herramientas.  

## Soluciones tradicionales de automatización y testing

### 1. Selenium

Selenium se ha consolidado como una de las referencias históricas en automatización de navegadores. Su principal fortaleza es la flexibilidad y el amplio ecosistema que lo rodea, lo que lo convierte en una herramienta muy extendida para pruebas web.  
Este requiere de un esfuerzo notable de configuración y mantenimiento.  
Pero eso hace que, no resuelva por sí mismo los problemas de análisis documental y estructuración de escenarios.  

### 2. Cypress

Cypress es una herramienta moderna orientada a pruebas end-to-end y de componentes en aplicaciones web. Destaca por su integración con el entorno de desarrollo, su facilidad de uso y su capacidad para observar la ejecución de pruebas de forma visual.  
En el contexto de CIC, Cypress forma parte del ecosistema real de trabajo. En el presente TFG no se llegará a implementar, pero si que se quiere implementar a nivel de empresa.  

### 3. JUnit y TestNG

Son marcos de prueba ampliamente utilizados en el ecosistema Java para la definición y ejecución de pruebas unitarias e integradas. Aportan estructura, anotaciones y capacidad de organización, siendo herramientas muy habituales en procesos de desarrollo con fuerte componente backend.  

### 4. Playwright

Playwright ha ganado relevancia por su enfoque moderno de automatización web, su soporte para múltiples navegadores y sus capacidades de depuración y espera automática. Estas características lo convierten en una opción muy atractiva para pruebas sobre interfaces dinámicas.  
Aun así, como ocurre con otras herramientas de automatización, su foco principal está en la ejecución de pruebas, no en la fase previa de interpretación documental y construcción estructurada de escenarios.  

### 5. Kiwi TCMS

Kiwi TCMS es una herramienta de gestión de pruebas de código abierto que permite definir casos, agruparlos en planes de prueba, registrar ejecuciones y mantener trazabilidad sobre el proceso de validación. Su interés en este trabajo es especialmente alto porque puede actuar como punto de destino de los scenarios generados por el sistema multiagente.  
Además, el hecho de contar con API facilita su integración con arquitecturas basadas en herramientas y automatización, lo que la convierte en un elemento especialmente adecuado para la propuesta concreta de este TFG.  

## Herramientas de testing basadas en IA

### 1. Testim

Testim es una plataforma orientada a la automatización de pruebas con capacidades de IA que ayudan a mejorar la estabilidad y reducir el mantenimiento. 
Su propuesta se centra en absorber parte del impacto de cambios frecuentes en la interfaz.  

### 2. Applitools

Applitools se orienta a la detección de regresiones visuales mediante Visual AI, permitiendo identificar diferencias perceptibles para el usuario en distintos navegadores y dispositivos. Este enfoque resulta especialmente potente en validaciones visuales complejas.  

### 3. Mabl

Mabl busca unificar creación, ejecución y análisis de pruebas web y API dentro de entornos guiados, incorporando capacidades de IA para hacer el proceso más asistido. Su enfoque facilita determinadas tareas operativas y de mantenimiento.  

### 4. Functionize

Functionize plantea una automatización empresarial apoyada en IA y capacidades cercanas a enfoques agénticos para acelerar la creación, mantenimiento y ejecución de flujos end-to-end.  

## Frameworks para el desarrollo de agentes

### 1. Google ADK

Google ADK es un framework orientado al desarrollo de agentes de IA, con capacidad para construir soluciones modulares, estructuradas y orientadas a procesos. Su interés está en la facilidad para crear arquitecturas en las que varios componentes colaboran dentro de un flujo definido. En su documentación se explica todo muy detalladamente y es fácil de seguir.  

### 2. LangGraph

LangGraph se orienta a construir aplicaciones stateful y multi-actor basadas en grafos, con especial atención a la persistencia, la orquestación y la trazabilidad de flujos largos. Su diseño resulta interesante para procesos en los que el estado y la secuencia de los pasos son críticos.  

### 3. AutoGen

AutoGen ha sido una referencia importante en el desarrollo de aplicaciones basadas en conversaciones entre agentes y en la experimentación con arquitecturas colaborativas.  
Sin embargo, este framework en concreto dependiendo del tipo de solución, puede resultar menos alineado que otros enfoques más orientados a procesos.  

### 4. CrewAI

CrewAI se centra en la orquestación de agentes colaborativos y flujos complejos, ofreciendo abstracciones de alto nivel para modelar equipos de agentes con roles definidos. Esta orientación resulta útil cuando se desea construir sistemas con separación clara de responsabilidades.  

| Criterio | Google ADK | LangGraph | AutoGen | CrewAI |
|---|---|---|---|---|
| Soporte multiagente | SI | SI | SI | SI |
| Flujos estructurados / orientados a proceso | SI | SI | NO | SI |
| Gestión fuerte de estado / persistencia | NO | SI | NO | SI |
| Enfoque principalmente conversacional | NO | NO | SI | NO |
| Encaje directo con este TFG | SI | SI | NO | SI |

En este trabajo se utiliza Google ADK no porque se considere necesariamente el mejor framework en términos generales, sino porque es la tecnología indicada por CIC Consulting Informático dentro del contexto empresarial en el que se desarrolla el TFG.  
A partir de esa decisión de entorno, Google ADK es un buen framework para realizar este trabajo, ya que ofrece soporte para arquitecturas multiagente y flujos estructurados.