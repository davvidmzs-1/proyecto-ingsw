# Sistema de Gestión de Reservas y Ocupación para Motel — Trabajo Práctico Integrador

Este repositorio contiene el análisis y diseño del sistema **Sistema de Gestión de Reservas y Ocupación para Motel**, desarrollado como Trabajo Práctico Integrador de la asignatura **Ingeniería de Software**.

El sitio publicado en GitHub Pages es la entrega oficial del trabajo. **No se envían archivos impresos ni copias por otros medios.**

🔗 **Sitio publicado:** `https://davvidmzs-1.github.io/proyecto-ingsw/`

---

## Integrantes del grupo

| Nombre completo | Rol / Responsabilidad principal | Usuario de GitHub |
|---|---|---|
| Francisco David Martínez Salinas | Desarrollo técnico y diseño del sistema | [@davvidmzs-1](https://github.com/davvidmzs-1) |
| Jonathan Fabrizio Urán Aguilera | Análisis de requisitos | [@bxomau](https://github.com/bxomau) |
| Aquiles Augusto Vera Salinas | Modelado y diagramas | [@Agussv89](https://github.com/Agussv89) |
| Blas Arnaldo Páez Sosa | Documentación y ejercitarios | [@blasarnaldopaezsosa-glitch](https://github.com/blasarnaldopaezsosa-glitch) |

## Usuario / cliente real

**Motel Piel con Piel** — negocio de alojamiento por horas ubicado en Paraguarí, que actualmente gestiona la disponibilidad de habitaciones y el registro de ingresos de forma manual (a mano o de palabra en recepción), lo que genera errores de doble ocupación y dificulta llevar un control claro de tarifas y horarios.

## Metodología de diseño y desarrollo elegida

**Modelado dirigido por UML sobre un proceso iterativo incremental.**

Elegimos este enfoque porque el sistema tiene un dominio acotado y bien delimitado (habitaciones, reservas, ingresos, tarifas), lo que permite avanzar por etapas —tal como pide el TP en sus tres entregas— refinando el modelo en cada iteración sin necesidad de definir todo el diseño de una sola vez. Además, UML nos da un lenguaje común para representar tanto el flujo de reserva anticipada como el de check-in inmediato dentro del mismo modelo.

---

## Entregas

| Entrega | Estado | Enlace |
|---|---|---|
| 1. Conceptualización | ✅ Entregado | [Ver documento](docs/conceptualizacion.md) |
| 2. Análisis | 🔲 Pendiente | [Ver documento](docs/analisis.md) |
| 3. Diseño | 🔲 Pendiente | [Ver documento](docs/diseno.md) |

## Estructura del repositorio

```
/docs           → contenido publicado en GitHub Pages (este es el sitio oficial de entrega)
  ├─ index.md          → página principal del sitio
  ├─ conceptualizacion.md
  ├─ analisis.md
  └─ diseno.md
/ejercitarios   → respuestas grupales a los ejercitarios de cada unidad
```

## Cómo publicar este sitio en GitHub Pages

Ya está configurado: GitHub Pages sirve el sitio desde la carpeta `/docs` de la rama `main`. Cada `push` a esa rama actualiza el sitio automáticamente en `https://davvidmzs-1.github.io/proyecto-ingsw/` en unos minutos, sin necesidad de reconfigurar nada.