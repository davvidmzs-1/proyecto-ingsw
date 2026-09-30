# Respuestas — Ejercitario Unidad 04

---

## Tema 1 · El proceso de requerimientos

**1. Define en tus propias palabras qué es la ingeniería de requerimientos.**

_Respuesta:_ La ingeniería de requerimientos es el proceso sistemático de descubrir, analizar, documentar y verificar qué es lo que un sistema de software debe hacer, y bajo qué condiciones debe hacerlo, trabajando junto a los usuarios y demás interesados. No es simplemente "anotar lo que el cliente pide", sino un trabajo de análisis para asegurar que lo que se documenta sea completo, claro y realmente resuelva el problema del negocio.

**2. Diferencia entre "requerimiento", "especificación de requisitos" e "ingeniería de requisitos", con un ejemplo de cada uno.**

_Respuesta:_ Un requerimiento es una necesidad puntual del sistema, por ejemplo: "el sistema debe permitir registrar el ingreso de un cliente sin reserva previa". La especificación de requisitos es el documento completo y organizado que reúne todos los requerimientos del sistema, como el archivo `analisis.md` que vamos a publicar en la Entrega 2 del TP. La ingeniería de requisitos es todo el proceso que lleva a producir esa especificación: entrevistar al usuario real del motel, analizar sus respuestas, redactar los requerimientos y validarlos con él.

---

## Tema 2 · Tipos de requerimientos

**3. Ejercicio de relación**

- A → 2
- B → 3
- C → 1

**4. Cuadro — requerimientos de usuario vs. requerimientos de sistema**

| Aspecto | Requerimientos de usuario | Requerimientos de sistema |
| --- | --- | --- |
| Audiencia principal | Clientes, usuarios finales y gerentes del negocio, sin conocimiento técnico. | Desarrolladores, arquitectos y equipo técnico que construye el sistema. |
| Nivel de detalle | General y de alto nivel, describiendo qué necesita el negocio. | Detallado y preciso, especificando exactamente cómo debe comportarse cada función. |
| Lenguaje utilizado | Lenguaje natural, cercano al vocabulario del negocio. | Lenguaje técnico y estructurado, muchas veces con notación formal (UML, pseudocódigo). |

**5. Ejemplo propio de requerimiento funcional y no funcional (sistema de reservas del motel).**

_Respuesta:_ Funcional: "El sistema debe permitir registrar el check-in de una habitación indicando el horario de ingreso y calculando automáticamente el horario límite según la tarifa seleccionada." No funcional: "El sistema debe mostrar el estado actualizado de todas las habitaciones en no más de 2 segundos, para no demorar la atención en recepción."

---

## Tema 3 · Características de los requerimientos

**6. Cuadro — pregunta que verifica cada característica**

| Característica | Pregunta que permite verificarla |
| --- | --- |
| Correcto | ¿Este requerimiento describe realmente algo que el sistema debe hacer, según lo acordado con el usuario? |
| No ambiguo | ¿Existe una única interpretación posible de este requerimiento, sin dar lugar a lecturas distintas? |
| Completo | ¿Están incluidas todas las funciones y condiciones necesarias, sin dejar huecos que deban suponerse? |
| Verificable | ¿Existe una forma objetiva de comprobar, mediante una prueba, si el sistema cumple o no este requerimiento? |

**7. Reescribí "El sistema debe ser rápido" para que cumpla las características de un buen requerimiento.**

_Respuesta:_ "El sistema debe mostrar el listado de habitaciones disponibles en un tiempo no mayor a 2 segundos, incluso con las 20 habitaciones del motel cargadas simultáneamente." Esta versión es verificable (se puede medir el tiempo), no ambigua (da un número concreto) y completa (aclara bajo qué condición de carga se mide).

---

## Tema 4 · Obtención y análisis de requerimientos

**8. Enumera las cuatro etapas del ciclo de obtención y análisis de requerimientos.**

_Respuesta:_ 1) Descubrimiento de requerimientos, 2) Clasificación y organización, 3) Priorización y negociación, 4) Especificación (documentación de los requerimientos).

**9. Ejercicio de relación**

- A → 3
- B → 1
- C → 2

---

## Tema 5 · Técnicas de especificación de requerimientos

**10-11. Cuadro — ventaja y limitación de cada técnica**

| Técnica | Ventaja | Limitación |
| --- | --- | --- |
| Lenguaje natural estructurado | Es fácil de entender para el cliente y los interesados no técnicos. | Puede volverse ambiguo o inconsistente si no se sigue una plantilla estricta. |
| Casos de uso | Describe con claridad la interacción entre el usuario y el sistema, incluyendo flujos alternativos. | No captura bien los requerimientos no funcionales ni las reglas de negocio complejas. |
| Historias de usuario | Son simples, rápidas de escribir y fáciles de priorizar en un backlog ágil. | Suelen carecer del detalle necesario para sistemas con reglas de negocio complejas, requiriendo criterios de aceptación adicionales. |
| Diagramas (UML) | Permiten visualizar relaciones y estructuras que serían difíciles de describir solo con texto. | Requieren que quien los lee conozca la notación, lo cual puede excluir a interesados no técnicos. |

---

## Tema 6 · Especificaciones formales

**11. ¿Qué es una especificación formal y en qué tipo de sistemas se justifica su uso?**

_Respuesta:_ Una especificación formal es una descripción de los requerimientos escrita con una notación matemática precisa, que permite verificar de forma rigurosa (incluso automatizada) que el sistema cumple ciertas propiedades, eliminando la ambigüedad del lenguaje natural. Se justifica en sistemas críticos donde un error puede tener consecuencias graves, como sistemas de control de tráfico aéreo, software médico que regula la dosis de un equipo, o sistemas bancarios que gestionan transacciones a gran escala.

---

## Tema 7 · Prototipado de los requerimientos

**12. Diferencia entre prototipo desechable y prototipo evolutivo, con un ejemplo de cada uno.**

_Respuesta:_ Un prototipo desechable se construye rápido y con poca calidad de código solo para validar una idea o mostrarle algo al cliente, y luego se descarta por completo: por ejemplo, armar unas pantallas de ejemplo en HTML estático solo para acordar el flujo de reserva del motel con el dueño. Un prototipo evolutivo, en cambio, se construye con buenas prácticas desde el inicio porque la intención es seguir mejorándolo hasta convertirlo en el sistema final, como ir desarrollando el módulo de reservas del motel directamente sobre el stack definitivo (Laravel + MySQL) e ir agregándole funcionalidades.

---

## Tema 8 · Técnicas de construcción rápida

**13. Menciona dos técnicas de construcción rápida de prototipos.**

_Respuesta:_ Desarrollo con lenguajes o frameworks de alto nivel: usar herramientas que permiten armar pantallas y lógica básica muy rápido (por ejemplo, un framework como Laravel con scaffolding automático de CRUDs) para tener algo funcional en poco tiempo. Reutilización de componentes existentes: aprovechar bibliotecas, paquetes o módulos ya hechos (por ejemplo, un paquete de gestión de reservas o de calendarios) en lugar de programar todo desde cero, acelerando la construcción del prototipo.

---

## Tema 9 · Validación de requerimientos

**14. Cuadro — técnica de validación y qué problema detecta mejor**

| Técnica de validación | Qué tipo de problema detecta mejor |
| --- | --- |
| Revisiones de requisitos | Detecta ambigüedades, contradicciones y omisiones en el texto de los requerimientos, antes de construir nada. |
| Prototipado | Detecta que el usuario en realidad necesitaba algo distinto a lo que se especificó, al mostrarle algo tangible con lo que interactuar. |
| Generación de casos de prueba | Detecta requerimientos que no son verificables, porque si no se puede escribir una prueba objetiva para un requerimiento, es señal de que está mal redactado. |

---

## Tema 10 · Administración de requerimientos

**15. ¿Qué es la trazabilidad de requerimientos y por qué es importante?**

_Respuesta:_ La trazabilidad de requerimientos es la capacidad de seguir el rastro de un requerimiento a lo largo de todo el proyecto: de dónde salió, qué diseño lo implementa, qué código lo construye y qué prueba lo verifica. Es importante porque permite saber, ante un cambio, qué partes del sistema se ven afectadas, y asegura que ningún requerimiento quede sin cubrir ni se implemente algo que nadie pidió — en nuestro TP, es justamente lo que se pide construir en la "matriz de trazabilidad" de la Entrega 2.

---

## Tema 11 · Medición de requerimientos

**16. Menciona dos métricas de requerimientos y qué información aporta cada una.**

_Respuesta:_ Cantidad de requerimientos que cambiaron después de ser aprobados: le indica al equipo qué tan estable (o volátil) es el entendimiento del problema, y si conviene revisar el proceso de obtención de requisitos. Porcentaje de requerimientos verificados mediante pruebas: le muestra al equipo qué proporción del sistema ya tiene una forma objetiva de comprobar que funciona correctamente, y cuánto trabajo de validación falta.

**17. Reflexión final.**

_Respuesta:_ Para nuestro sistema de reservas del motel usaría entrevistas como técnica de obtención, porque el usuario real (el encargado del motel) puede explicar en detalle cómo maneja hoy la ocupación y qué le genera problemas, algo que sería difícil de captar solo con observación. Como técnica de especificación usaría casos de uso, porque el sistema tiene dos flujos bien diferenciados (reserva anticipada y check-in inmediato) que se describen mejor mostrando la interacción paso a paso que con una simple lista de historias de usuario. Y como técnica de validación usaría prototipado, mostrándole al encargado del motel unas pantallas de ejemplo del flujo de check-in antes de construir el sistema completo, porque es una persona sin perfil técnico y necesita ver algo concreto para poder confirmar si entendimos bien su forma de trabajar.
