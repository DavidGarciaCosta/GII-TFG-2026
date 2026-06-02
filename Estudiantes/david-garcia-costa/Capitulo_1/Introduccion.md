# Introducción

El capítulo de Introducción se entiende como una breve presentación del tema del TFG, una idea somera pero concisa de los diferentes aspectos de los que se compone el trabajo, así como de las implicaciones que puede tener en la comunidad científica o en la práctica profesional.

## Motivación

En este Trabajo de Fin de Grado se propone realizar un diseño e implementar una aplicación web manual con un sistema de agentes de Inteligencia Artificial orientado a mejorar el proceso de testing de QA de CIC Consulting Informático.

La motivación que lleva a realizar este trabajo sale de una necesidad por parte de CIC. Actualmente, el esfuerzo de los ingenieros de QA está en hacer tareas de elevada carga; como puede ser la interpretación de documentación (Documentos de Requisitos Funcionales y Documentos de Diseño del Sistema), el análisis de los requisitos funcionales y casos de uso que contienen dichos documentos, la redacción manual de planes de prueba dentro de un Excel, en Kiwi TCMS ahora mismo solo hay unos cuantos ejemplos de los escenarios en lenguaje Gherkin y están dentro de una carpeta de VSCode donde trabaja el ingeniero, no están en ninguna API. Estas actividades requieren considerable inversión de tiempo y conocimiento especializado, lo que limita la escalabilidad del proceso y genera dependencia.

## Problemática Identificada

En términos más específicos, se puede decir que el flujo de trabajo actual en CIC presenta las siguientes limitaciones:

- Dependencia del análisis manual
- Falta de automatización en fase de análisis
- Escalabilidad limitada
- Trazabilidad mejorable

## Propuesta de Solución

El presente trabajo plantea como primera aproximación el desarrollo de una aplicación con posibilidad de realizarlo de forma manual o automatizado con agentes de Inteligencia Artificial que ayuden al equipo de QA en las tareas previas a la creación y publicación de casos de prueba. La idea principal es que la aplicación pueda recibir documentación funcional, analizar su contenido y proponer una estructura inicial de requisitos, casos de uso, escenarios de prueba y borrador para caso de prueba.

La solución se concibe como un flujo dividido en tareas especializadas. Un agente podría encargarse de interpretar la documentación de entrada y localizar los elementos relevantes; otro podría transformar esa información en escenarios de prueba en lenguaje Gherkin; y otro podría preparar una propuesta revisable antes de que el equipo decida si debe incorporarse al sistema de gestión de pruebas.

Esta propuesta no busca sustituir completamente la intervención del equipo de QA, sino servir como herramienta de apoyo. El objetivo es reducir tareas repetitivas, estructurar mejor la información y mantener siempre una revisión humana antes de que los casos de prueba sean considerados válidos. De esta forma, el proyecto plantea un prototipo controlado que permita comprobar si este enfoque es viable y útil dentro de un contexto real.

---

[← Volver al Índice](../README.md)
