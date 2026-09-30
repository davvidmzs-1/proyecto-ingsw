# Respuestas — Ejercitario Unidad 03

---

## Tema 1 · El significado de proceso

**1. Define en tus propias palabras qué es un proceso de software.**

_Respuesta:_ Un proceso de software es el conjunto ordenado de actividades, técnicas y prácticas que un equipo sigue para producir un sistema de software, desde que se entiende el problema hasta que el producto se entrega y se mantiene. No es una receta rígida sino un marco de trabajo que organiza cuándo y cómo se hacen las cosas para llegar a un resultado de calidad de forma predecible.

**2. Explica la diferencia entre proceso, metodología y modelo de proceso, con un ejemplo de cada uno.**

_Respuesta:_ El proceso es el marco general de actividades que se deben cumplir (por ejemplo, especificar, diseñar, construir y validar). La metodología es el conjunto concreto de técnicas, notaciones y prácticas paso a paso con las que se ejecuta ese proceso (por ejemplo, Scrum, que define sprints, roles y ceremonias concretas). El modelo de proceso es la representación abstracta de cómo se organizan esas actividades en el tiempo (por ejemplo, el modelo en cascada, que las ordena de forma estrictamente secuencial).

**3. Enumera las cinco actividades genéricas del marco de trabajo de Pressman.**

_Respuesta:_ 1) Comunicación, 2) Planeación, 3) Modelado, 4) Construcción, 5) Despliegue.

**4. Menciona dos actividades "de la sombrilla" y explica por qué se dice que "cubren" todo el proceso.**

_Respuesta:_ Dos ejemplos son la gestión de riesgos y el aseguramiento de la calidad. Se llaman "de la sombrilla" porque no ocurren en un momento puntual del proceso, sino que se aplican de forma continua a lo largo de todas las actividades genéricas, desde la comunicación inicial hasta el despliegue, protegiendo al proyecto como una sombrilla cubre todo lo que está debajo.

---

## Tema 2 · Modelos de proceso

**5. Cuadro — ¿Cuándo conviene usar cada modelo?**

| Modelo | ¿Cuándo conviene usarlo? |
| --- | --- |
| Cascada | Cuando los requisitos están claros, completos y no se espera que cambien durante el desarrollo. |
| Incremental | Cuando se necesita entregar funcionalidad útil de forma temprana y el proyecto puede dividirse en partes independientes. |
| Evolutivo (prototipos) | Cuando el cliente no tiene claros sus requisitos y necesita ver algo funcionando para poder definirlos. |
| Evolutivo (espiral) | Cuando el proyecto es de alto riesgo o gran escala y se necesita evaluar riesgos en cada ciclo antes de avanzar. |
| Concurrente | Cuando distintas actividades del proyecto (diseño, codificación, pruebas) pueden y deben avanzar en paralelo, como en equipos con varios frentes de trabajo simultáneos. |

**6. Ejercicio de relación**

- A → 2
- B → 4
- C → 5
- D → 1
- E → 3

**7. Elegí un proyecto de software (hipotético o real) y justificá qué modelo de proceso usarías.**

_Respuesta:_ Para el sistema de reservas del motel que estamos desarrollando como Trabajo Práctico, usaríamos un modelo incremental. Esto es porque el sistema tiene módulos claramente separables (gestión de habitaciones, reservas, check-in/check-out, facturación) que pueden entregarse por partes funcionales, y porque nos permite ir validando cada módulo con el usuario real antes de avanzar al siguiente, reduciendo el riesgo de construir algo que no se ajuste a cómo trabaja el motel.

---

## Tema 3 · Iteración de procesos

**8. Explica con tus palabras por qué la mayoría de los procesos modernos son iterativos.**

_Respuesta:_ Porque rara vez se conocen todos los requisitos de un sistema desde el principio, y los procesos iterativos permiten construir, mostrar y corregir en ciclos cortos en lugar de esperar hasta el final para descubrir errores de interpretación. Esto reduce el riesgo de invertir mucho tiempo en una dirección equivocada y facilita adaptarse a cambios que van surgiendo durante el desarrollo.

**9. Menciona una ventaja y una desventaja de trabajar con iteraciones cortas.**

_Respuesta:_ Ventaja: permiten detectar errores y malentendidos de forma temprana, ya que el cliente ve resultados concretos cada poco tiempo y puede corregir el rumbo antes de que el problema se agrande. Desventaja: exigen una comunicación constante con el cliente y el equipo, lo cual puede ser difícil de sostener si el cliente no tiene disponibilidad frecuente, o generar sobrecarga de reuniones y revisiones.

---

## Tema 4 · Especificación, diseño, implementación, validación y evolución

**10. Cuadro — Qué implica cada actividad fundamental (Sommerville)**

| Actividad | Qué implica |
| --- | --- |
| Especificación | Definir qué debe hacer el sistema y bajo qué restricciones debe operar, en conjunto con los clientes e interesados. |
| Diseño e implementación | Transformar la especificación en un sistema que efectivamente funcione, tomando decisiones de arquitectura y escribiendo el código. |
| Validación | Comprobar que el sistema construido realmente cumple lo que el cliente necesita y que hace lo que se especificó. |
| Evolución | Modificar el sistema en el tiempo para adaptarlo a nuevas necesidades del negocio, corregir errores o incorporar mejoras. |

**11. Relación con las cinco fases del ciclo del software (Unidad 1).**

_Respuesta:_ Se parecen en que ambas describen el mismo recorrido general: primero se entiende qué se necesita, después se construye y se comprueba que funcione, y finalmente el sistema sigue viviendo y cambiando en el tiempo. Se diferencian en el nivel de detalle: el ciclo de Sommerville agrupa diseño e implementación en una sola actividad, mientras que el ciclo de vida clásico de la Unidad 1 las separa en fases distintas (análisis, diseño, implementación, pruebas, mantenimiento); además, Sommerville junta las pruebas dentro de "validación" en lugar de tratarlas como una fase aparte.

---

## Tema 5 · Herramientas y técnicas para modelado de procesos

**12. Menciona dos formas de representar un proceso (no un sistema) y explica brevemente cada una.**

_Respuesta:_ Diagramas de flujo de proceso: representan gráficamente las actividades del proceso y el orden en que se ejecutan, usando cajas y flechas que muestran la secuencia y las decisiones. Descripciones basadas en roles: se documenta el proceso indicando qué rol es responsable de cada actividad y qué entregable produce, en lugar de solo el orden temporal de las tareas.

**13. ¿Qué es un patrón de proceso? Da un ejemplo hipotético.**

_Respuesta:_ Un patrón de proceso es una solución probada y reutilizable para un problema recurrente que ocurre durante el desarrollo de software, similar a los patrones de diseño pero aplicado a la forma de trabajar del equipo, no al código. Ejemplo hipotético: en un proyecto los requisitos cambian constantemente porque el cliente no tiene claro lo que quiere; el patrón de proceso "prototipado rápido con validación temprana" resuelve esto construyendo una versión simplificada del sistema para que el cliente la pruebe antes de comprometerse con requisitos definitivos.

---

## Tema 6 · Ayuda automatizada al proceso

**14. Explica la diferencia entre herramientas Upper-CASE y Lower-CASE.**

_Respuesta:_ Las herramientas Upper-CASE dan soporte a las primeras etapas del proceso: análisis, especificación y diseño de alto nivel (por ejemplo, herramientas para dibujar diagramas UML o modelar requisitos). Las herramientas Lower-CASE dan soporte a las etapas posteriores, más cercanas a la construcción: generación de código, pruebas y depuración.

**15. Menciona tres herramientas CASE y clasifícalas.**

| Herramienta | Categoría |
| --- | --- |
| Draw.io / Lucidchart (diagramas UML) | Upper-CASE |
| Visual Studio Code (editor con depurador integrado) | Lower-CASE |
| Visual Paradigm (modelado + generación de código) | I-CASE |

**16. Reflexión final.**

_Respuesta:_ Para un proyecto personal elegiría un modelo incremental. Al ser un proyecto chico y con tiempo limitado (materias en paralelo, como es nuestro caso), no me conviene un modelo en cascada porque no tengo forma de validar los requisitos de una sola vez con certeza total; en cambio, entregar el proyecto en partes pequeñas y funcionales me permite corregir el rumbo sin haber invertido todo el tiempo disponible en una sola etapa larga.
