# Respuestas — Ejercitario Unidad 01

---

## Tema 1 · Ingeniería de software: una visión previa

**1. En tus propias palabras, define qué es la Ingeniería de Software.**

_Respuesta:_ La Ingeniería de Software es la disciplina que aplica principios, métodos y herramientas de ingeniería para diseñar, construir, probar y mantener sistemas de software de forma sistemática y controlada. No se limita a escribir código: abarca todo el proceso, desde entender el problema del usuario hasta entregar y sostener una solución confiable a lo largo del tiempo. Su objetivo es producir software de calidad dentro de plazos y presupuestos realistas.

**2. Explica con un ejemplo la diferencia entre "programar" y "hacer ingeniería de software".**

_Respuesta:_ Programar es escribir el código que resuelve una tarea puntual, por ejemplo un script que ordena una lista de números. Hacer ingeniería de software implica además analizar los requisitos del usuario, diseñar la arquitectura del sistema, documentar decisiones, escribir pruebas y planificar el mantenimiento futuro. Por ejemplo, crear un sistema de turnos para una clínica no es solo programar el formulario de reserva: implica modelar el flujo completo, prever errores, definir roles de usuario y asegurar que el sistema siga funcionando cuando cambien los requisitos.

**3. Menciona dos razones por las cuales la ingeniería de software es necesaria en el desarrollo de sistemas actuales.**

_Respuesta:_ Primero, los sistemas actuales son cada vez más complejos y suelen integrar múltiples componentes (bases de datos, APIs, servicios externos), por lo que sin un proceso ordenado es fácil que el proyecto se vuelva inmanejable. Segundo, el software moderno maneja información crítica y datos de usuarios reales, así que se necesita un proceso disciplinado que garantice calidad, seguridad y mantenibilidad a largo plazo.

---

## Tema 2 · El rol de la IS en el diseño de sistemas (+ impacto de la IA)

**4. Enumera los elementos que conforman un sistema basado en computadora, además del software.**

_Respuesta:_ Hardware, personas (usuarios y operadores), bases de datos, documentación y procedimientos, y en muchos casos también las redes de comunicación que conectan a los distintos componentes.

**5. Describe brevemente la diferencia entre una visión sistémica y una visión aislada del software en el diseño de sistemas.**

_Respuesta:_ Una visión aislada trata al software como un producto independiente, enfocándose solo en su funcionamiento interno. Una visión sistémica lo entiende como una pieza dentro de un sistema más grande, que interactúa con hardware, personas y otros procesos; los cambios en cualquiera de esas partes afectan al resto. Por eso el diseño debe considerar el contexto completo y no solo el código.

**6. Elige una herramienta de inteligencia artificial aplicada al desarrollo de software e indica lo pedido.**

_Respuesta:_ Herramienta elegida: un asistente de código tipo GitHub Copilot.
- Tarea que apoya: la escritura y autocompletado de código, y la generación de pruebas unitarias básicas.
- Beneficio concreto: acelera tareas repetitivas y reduce el tiempo dedicado a código boilerplate, dejando más tiempo para el diseño y la resolución de problemas complejos.
- Riesgo o desafío: puede introducir código con errores sutiles o vulnerabilidades si el desarrollador no lo revisa críticamente, y existe el riesgo de que el equipo pierda comprensión profunda del código generado.

---

## Tema 3 · Historia de la Ingeniería de Software

_Relación evento–descripción:_

- A → 3
- B → 1
- C → 5
- D → 4
- E → 2

**7. En tu opinión, ¿por qué la "crisis del software" de 1968 marcó un punto de inflexión para la disciplina?**

_Respuesta:_ Porque expuso de forma pública que desarrollar software de manera artesanal, sin procesos ni estándares, generaba proyectos que se retrasaban, superaban ampliamente el presupuesto y fallaban en producción. Esto llevó a la comunidad a reconocer la necesidad de tratar el desarrollo de software con la misma rigurosidad que otras ramas de la ingeniería, dando origen formal a la disciplina.

---

## Tema 4 · El rol del ingeniero de software

**8. Menciona tres competencias que debe tener un ingeniero de software, además del conocimiento técnico.**

_Respuesta:_ Comunicación efectiva con clientes y equipos no técnicos, capacidad de trabajo en equipo, y pensamiento crítico para tomar decisiones de diseño bajo restricciones de tiempo y recursos.

**9. Describe brevemente qué hace cada rol dentro de un equipo de desarrollo.**

| Rol | Descripción |
| --- | --- |
| Analista | Releva y documenta los requisitos del sistema junto al usuario, traduciendo sus necesidades en especificaciones claras. |
| Arquitecto | Define la estructura general del sistema: cómo se organizan los componentes y cómo se comunican entre sí. |
| Desarrollador | Implementa el software siguiendo el diseño acordado, escribiendo y probando el código. |
| Tester / QA | Verifica que el sistema cumpla los requisitos y detecta errores antes de que lleguen al usuario final. |

**10. Caso breve: falla de seguridad cerca de la entrega.**

_Respuesta:_ Debería informar la falla al equipo y a los responsables del proyecto de inmediato, aunque eso implique retrasar la entrega. La ética profesional prioriza la seguridad y privacidad de los usuarios por sobre cumplir un plazo; entregar un sistema con una vulnerabilidad conocida sin corregirla ni informarla sería una falta grave de responsabilidad profesional y podría causar un daño real a terceros.

---

## Tema 5 · El ciclo del software

**11. Ordena y nombra las cinco fases genéricas del ciclo de vida del software.**

_Respuesta:_ 1) Análisis de requisitos, 2) Diseño, 3) Implementación (codificación), 4) Pruebas, 5) Mantenimiento.

**12. ¿Por qué el mantenimiento suele ser la fase más costosa? Da un ejemplo hipotético.**

_Respuesta:_ Porque el software permanece en uso durante años y en ese tiempo deben corregirse errores no detectados, adaptarse a nuevas necesidades del negocio y actualizarse por cambios tecnológicos, todo sobre una base de código ya existente que puede ser compleja de modificar sin romper otras partes. Por ejemplo, un sistema de facturación construido hace cinco años puede necesitar adaptarse a un cambio en la normativa impositiva, lo que obliga a revisar módulos que nadie tocaba desde su creación.

---

## Tema 6 · Relación con otras áreas de la Ciencia de la Computación

| Área | ¿Cómo apoya a la Ingeniería de Software? |
| --- | --- |
| Estructuras de datos y algoritmos | Proveen las bases para diseñar soluciones eficientes en tiempo y uso de memoria dentro del software. |
| Bases de datos | Permiten almacenar, organizar y recuperar la información que el sistema necesita de forma persistente y confiable. |
| Sistemas operativos | Ofrecen los servicios sobre los que corre el software (gestión de procesos, memoria, archivos) y condicionan su diseño. |
| Redes | Habilitan la comunicación entre componentes distribuidos, como en sistemas cliente-servidor o aplicaciones web. |

---

## Tema 7 · Relación con otras disciplinas

**13. Elige dos disciplinas y explica cómo se relacionan con el trabajo diario de un ingeniero de software.**

_Respuesta:_ Administración: un ingeniero de software suele coordinar tiempos, recursos y prioridades del proyecto, aplicando conceptos de gestión para cumplir plazos sin sacrificar calidad. Comunicación: gran parte del trabajo consiste en entender lo que el cliente necesita (que muchas veces no sabe expresar técnicamente) y explicar decisiones técnicas en términos que un usuario no técnico pueda comprender.

**14. Reflexión final: ¿qué idea te resultó más relevante y por qué?**

_Respuesta:_ La idea de que la ingeniería de software no es solo escribir código sino gestionar todo el ciclo de vida de un sistema, porque cambia la forma de encarar el Trabajo Práctico del semestre.]