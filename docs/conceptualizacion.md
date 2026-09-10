# Conceptualización

## Presentación del proyecto

**Nombre del sistema:** Sistema de Gestión de Reservas y Ocupación para Motel

**Integrantes:**
- Francisco David Martínez — Desarrollo técnico y diseño del sistema
- Fabrizio Urán — Análisis de requisitos
- Aquiles Augusto Vera — Modelado y diagramas

**Usuario/cliente real:** Motel Piel con Piel — negocio de alojamiento por horas ubicado en Paraguari, que actualmente gestiona la disponibilidad de habitaciones y el registro de ingresos de forma manual.

## Definición del problema

Actualmente el motel controla la ocupación de sus habitaciones de forma manual: el personal de recepción anota en papel o de memoria qué habitaciones están ocupadas y a qué hora vence cada estadía. Esto genera errores frecuentes de doble asignación de una misma habitación, dificultad para calcular el cobro exacto según el tiempo de uso, y falta de información centralizada para saber en tiempo real cuántas habitaciones están disponibles. Además, no queda un registro histórico ordenado que permita analizar la ocupación a lo largo del tiempo.

## Propósito y objetivos

**Objetivo general:** Desarrollar un sistema que permita gestionar de forma centralizada la disponibilidad, reserva y ocupación de las habitaciones del motel, reduciendo errores de asignación y agilizando el registro de ingresos.

**Objetivos específicos:**
- Permitir registrar reservas anticipadas de habitaciones.
- Permitir registrar el ingreso directo (walk-in) de un cliente sin reserva previa.
- Mostrar en todo momento el estado de ocupación de cada habitación (libre, ocupada, en limpieza).
- Calcular automáticamente el monto a cobrar según el tiempo de permanencia y la tarifa vigente.
- Llevar un historial de ocupación por habitación.

## Alcance del proyecto

**Incluye (primera versión):**
- Gestión de habitaciones y su estado (libre / ocupada / en limpieza).
- Registro de reservas anticipadas.
- Registro de check-in inmediato (walk-in).
- Cálculo de tarifa según franja horaria y tiempo de estadía.
- Registro de check-out.

**Fuera de alcance (por ahora):**
- Pagos en línea o pasarelas de pago.
- Aplicación móvil para clientes.
- Facturación electrónica ante organismos fiscales.
- Múltiples sucursales.

## Interesados (stakeholders)

| Interesado | Interés en el proyecto |
| --- | --- |
| Dueño/encargado del motel | Reducir errores de asignación y tener control de la ocupación y los ingresos. |
| Personal de recepción | Contar con una herramienta simple y rápida para registrar ingresos y consultar disponibilidad. |
| Cliente | Poder reservar con anticipación cuando lo necesite, o ser atendido rápido al llegar sin reserva. |
| Grupo de desarrollo (cátedra) | Evaluar el correcto análisis y diseño del sistema como Trabajo Práctico Integrador. |

## Justificación / viabilidad

- **Técnica:** el dominio del problema es acotado (habitaciones, reservas, tarifas), lo que permite construir un sistema funcional con tecnologías web estándar dentro del tiempo del cuatrimestre.
- **Operativa:** el personal ya realiza estas tareas manualmente; el sistema digitaliza un proceso existente sin cambiar la forma de trabajo del motel.
- **Económica:** al ser un sistema de alcance acotado, no requiere infraestructura costosa; puede alojarse en un hosting básico o incluso ejecutarse localmente en la recepción.

## Visión general de la solución

El sistema tendrá un panel donde el personal de recepción vea el estado de todas las habitaciones. Desde ahí podrá registrar una reserva anticipada (indicando fecha/hora prevista) o dar de alta un ingreso inmediato. Al finalizar la estadía, el sistema calculará el monto según el tiempo transcurrido y la tarifa correspondiente, y liberará la habitación para el siguiente uso.

## Glosario de términos

- **Habitación:** unidad de alojamiento que puede reservarse u ocuparse, con una tarifa asociada.
- **Reserva:** solicitud registrada con anticipación para ocupar una habitación en una fecha/hora futura.
- **Check-in:** momento en que un cliente ingresa efectivamente a una habitación, con o sin reserva previa.
- **Check-out:** momento en que el cliente desocupa la habitación y finaliza el cobro.
- **Walk-in:** cliente que se presenta sin reserva previa y solicita una habitación en el momento.
- **Tarifa por franja horaria:** precio asociado a un rango de tiempo de uso de la habitación.
- **Estado de habitación:** condición actual de una habitación (libre, ocupada, en limpieza).

## Riesgos iniciales

| Riesgo | Mitigación |
| --- | --- |
| Dificultad para conseguir acceso real al usuario/cliente (motel) durante todo el cuatrimestre. | Mantener contacto temprano y frecuente; tener un perfil de usuario alternativo definido en caso de no conseguir uno real. |
| Alcance mal definido entre "reserva" y "walk-in" puede complejizar el modelo. | Definir claramente ambos flujos desde esta etapa y mantenerlos separados pero coherentes. |
| Tiempo limitado del grupo (materias en paralelo). | Priorizar funcionalidades core antes de agregar extras. |

## Selección tecnológica preliminar

- **Lenguaje:** PHP.
- **Framework:** Laravel.
- **Base de datos:** MySQL.

Justificación: el grupo ya tiene experiencia previa con este stack, lo que reduce el riesgo técnico y permite enfocar el tiempo disponible en el análisis y diseño del dominio en lugar de en aprender herramientas nuevas.