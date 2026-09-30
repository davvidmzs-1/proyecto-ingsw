# Respuestas — Ejercitario Unidad 02

---

## Tema 1 · Propiedades de los sistemas

**1. Define en tus propias palabras qué es un sistema y da un ejemplo distinto al utilizado en clase.**

_Respuesta:_ Un sistema es un conjunto de elementos interrelacionados que trabajan juntos para lograr un objetivo común, de forma que el resultado de esa interacción es distinto a lo que cada elemento podría producir por separado. Un ejemplo distinto al de clase sería un sistema de transporte público urbano: buses, paradas, choferes, horarios y usuarios interactúan entre sí para cumplir el objetivo de trasladar personas por la ciudad.

**2. Enumera los seis elementos de un sistema basado en computadora.**

_Respuesta:_ Software, hardware, personas, bases de datos, documentación y procedimientos.

**3. Sistema cotidiano — tabla de propiedades (elegido: un supermercado)**

| Propiedad | Ejemplo en el sistema elegido |
|---|---|
| Jerarquía | El supermercado se organiza en subsistemas como cajas, góndolas, depósito y administración, cada uno con sus propias reglas internas. |
| Límites (fronteras) | El límite del sistema es el propio local: lo que ocurre dentro (reposición, cobro, atención) es parte del sistema, mientras que el proveedor externo que entrega la mercadería queda fuera de esa frontera. |
| Interrelación de elementos | Si el sistema de cajas se cae, no se puede cobrar, y eso afecta directamente al depósito porque no se libera espacio de stock vendido. |
| Propiedades emergentes | La "experiencia de compra" (rapidez, orden, disponibilidad de productos) surge de la combinación de todos los subsistemas funcionando bien juntos, no de uno solo. |

**4. Identifica un posible subsistema del mismo sistema y justifica por qué lo consideras tal.**

_Respuesta:_ El subsistema de cajas registradoras. Lo considero un subsistema porque tiene sus propios elementos (cajeros, lectores de código de barras, terminal de pago), su propio proceso interno (escanear, cobrar, emitir ticket) y una función claramente delimitada dentro del sistema más grande del supermercado, pero depende de otros subsistemas (como el de inventario) para funcionar correctamente.

---

## Tema 2 · Los sistemas y su entorno

**5. Sistema de software habitual — entrada, salida y entorno**

| Elemento | Descripción en el sistema elegido |
|---|---|
| Sistema elegido | WhatsApp |
| Una entrada | El mensaje de texto que el usuario escribe y envía. |
| Una salida | La notificación push que recibe el destinatario en su celular. |
| Un elemento del entorno | La conexión a internet del dispositivo, que no es parte del sistema pero condiciona si puede funcionar. |

**6. ¿El sistema que elegiste es abierto o cerrado? Justifica tu respuesta.**

_Respuesta:_ Es un sistema abierto, porque interactúa constantemente con su entorno: depende de la red de internet, de los servidores externos de Meta, y de otros sistemas del teléfono (contactos, cámara, notificaciones) para funcionar. Un sistema cerrado no tendría ningún intercambio con el exterior una vez en funcionamiento, y ese no es el caso.

**7. Explica con tus palabras qué es la retroalimentación (feedback) en un sistema y da un ejemplo.**

_Respuesta:_ La retroalimentación es cuando la salida de un sistema (o parte de ella) se vuelve a usar como entrada para ajustar su propio comportamiento. Por ejemplo, en WhatsApp, cuando un mensaje falla en enviarse, el sistema detecta ese resultado (la salida "no se pudo enviar") y lo usa para mostrarle al usuario un ícono de error y reintentar el envío automáticamente.

**8. Restricción externa real que podría afectar al sistema elegido, indicando si es organizacional, regulatoria o tecnológica.**

_Respuesta:_ Una restricción regulatoria: las leyes de protección de datos personales de cada país (como el RGPD en Europa) obligan a WhatsApp a cifrar los mensajes y limitar qué datos puede almacenar o compartir sobre sus usuarios, condicionando directamente cómo se diseña el sistema.

---

## Tema 3 · Modelado de sistemas

**9. Menciona dos razones por las cuales es útil modelar un sistema antes de construirlo.**

_Respuesta:_ Primero, permite detectar errores de diseño o malentendidos con el cliente antes de invertir tiempo y dinero en construir algo equivocado. Segundo, facilita la comunicación entre los distintos interesados del proyecto (clientes, desarrolladores, analistas), ya que un modelo visual suele ser más fácil de entender y discutir que una descripción extensa en texto.

**10. Ejercicio de relación**

| Nivel de visión | Descripción |
|---|---|
| A. Visión del mundo (worldview) | 3 |
| B. Visión del dominio | 4 |
| C. Visión del elemento | 1 |
| D. Visión detallada | 2 |

**11. Explica la diferencia entre vista estructural y vista de comportamiento, y da un ejemplo de notación para cada una.**

_Respuesta:_ La vista estructural muestra cómo están organizados los componentes de un sistema y cómo se relacionan entre sí de forma estática, por ejemplo mediante un diagrama de clases UML. La vista de comportamiento, en cambio, muestra cómo el sistema actúa a lo largo del tiempo, es decir, la secuencia de acciones o el flujo de eventos, por ejemplo mediante un diagrama de secuencia UML.

**12. Diagrama de contexto.**

_Nota: este punto pide dibujar y adjuntar una imagen — no se puede completar en texto. Ejemplo de sistema sugerido: un cajero automático, con las entidades externas "Cliente" y "Banco central" interactuando con el sistema mediante flechas de entrada/salida (tarjeta e identificación por un lado, autorización de la transacción por el otro). Hagan el dibujo a mano o en una herramienta como draw.io y arrástrenlo al editor de GitHub para insertarlo en este punto._

**13. ¿En qué situación elegirías usar simulación en lugar de un modelo estático? Da un ejemplo concreto.**

_Respuesta:_ Elegiría simulación cuando necesito entender cómo se comporta el sistema a lo largo del tiempo bajo distintos escenarios, algo que un modelo estático no puede mostrar. Por ejemplo, para nuestro sistema del motel, simularía la ocupación de las habitaciones durante un fin de semana con alta demanda, para ver si el sistema soporta picos de reservas simultáneas antes de implementarlo realmente.

---

## Tema 4 · El proceso de Ingeniería de Sistemas

**14. Explica la diferencia entre Ingeniería de procesos de negocio e Ingeniería de producto, dando un ejemplo de cada una.**

_Respuesta:_ La Ingeniería de procesos de negocio se enfoca en rediseñar cómo opera una organización, sin que necesariamente el resultado sea un software; por ejemplo, reorganizar el flujo de atención al cliente de una empresa para reducir tiempos de espera. La Ingeniería de producto, en cambio, se enfoca en construir un sistema o producto concreto que cumpla ciertos requisitos técnicos; por ejemplo, desarrollar el sistema de reservas del motel que estamos construyendo como Trabajo Práctico.

**15. Ordena numéricamente (1 a 4) los siguientes pasos genéricos del proceso de Ingeniería de Sistemas.**

| N.º | Paso |
|---|---|
| 3 | Especificación del sistema |
| 1 | Definición de necesidades |
| 4 | Asignación de requisitos entre elementos |
| 2 | Análisis de factibilidad |

**16. Reflexión final: ¿por qué es importante que un ingeniero de software comprenda el sistema completo antes de programar?**

_Respuesta:_ Porque el software casi nunca funciona de forma aislada: interactúa con hardware, personas y procesos del negocio, y si el ingeniero solo se enfoca en el código sin entender ese contexto completo, corre el riesgo de construir una solución técnicamente correcta pero que no resuelve el problema real del usuario. Esto se relaciona directamente con la visión sistémica vista en la Unidad 01: así como ahí vimos que el software es solo una pieza de un sistema más grande, en esta unidad confirmamos que hay que entender primero cómo funciona ese sistema completo (como el motel en nuestro TP, con su recepción, sus horarios y sus reglas propias) antes de empezar a programar cualquier módulo.
