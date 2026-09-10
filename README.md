# Sistema de Gestión de Reservas y Ocupación para Motel — Trabajo Práctico Integrador

Este repositorio contiene el análisis y diseño del sistema **Sistema de Gestión de Reservas y Ocupación para Motel**, desarrollado como Trabajo Práctico Integrador de la asignatura **Ingeniería de Software**.

El sitio publicado en GitHub Pages es la entrega oficial del trabajo. **No se envían archivos impresos ni copias por otros medios.**

🔗 **Sitio publicado:** `https://davvidmzs-1.github.io/proyecto-ingsw/`

---

## Integrantes del grupo

| Nombre completo | Rol / Responsabilidad principal | Usuario de GitHub |
|---|---|---|
| Francisco David Martínez | Desarrollo técnico y diseño del sistema | [@davvidmzs-1] |
| Fabrizio Urán | Análisis de requisitos | [@usuario2] |
| Aquiles Augusto Vera | Modelado y diagramas | [@usuario3] |

## Usuario / cliente real

**Motel Piel con Piel** — negocio de alojamiento por horas que actualmente gestiona la disponibilidad de habitaciones y el registro de ingresos de forma manual (a mano o de palabra en recepción), lo que genera errores de doble ocupación y dificulta llevar un control claro de tarifas y horarios.

## Metodología de diseño y desarrollo elegida

**Modelado dirigido por UML sobre un proceso iterativo incremental.**

Elegimos este enfoque porque el sistema tiene un dominio acotado y bien delimitado (habitaciones, reservas, ingresos, tarifas), lo que permite avanzar por etapas —tal como pide el TP en sus tres entregas— refinando el modelo en cada iteración sin necesidad de definir todo el diseño de una sola vez. Además, UML nos da un lenguaje común para representar tanto el flujo de reserva anticipada como el de check-in inmediato dentro del mismo modelo.

---

## Entregas

| Entrega | Estado | Enlace |
|---|---|---|
| 1. Conceptualización | 🔲 Pendiente | [Ver documento](docs/conceptualizacion.md) |
| 2. Análisis | 🔲 Pendiente | [Ver documento](docs/analisis.md) |
| 3. Diseño | 🔲 Pendiente | [Ver documento](docs/diseno.md) |

## Estructura del repositorio

```
/docs           → contenido publicado en GitHub Pages (este es el sitio oficial de entrega)
  ├─ index.md          → página principal del sitio
  ├─ conceptualizacion.md
  ├─ analisis.md
  └─ diseno.md
/diagramas      → imágenes o archivos fuente de los diagramas (UML, mockups, etc.)
/src            → código fuente, si el grupo decide avanzar con una implementación
```

## Cómo publicar este sitio en GitHub Pages

1. Suban este repositorio a GitHub (público, o privado con acceso otorgado a la cátedra).
2. Vayan a **Settings → Pages**.
3. En **Source**, seleccionen la rama `main` (o `master`) y la carpeta **/docs**.
4. Guarden. GitHub publicará el sitio en `https://davvidmzs-1.github.io/proyecto-ingsw/` en unos minutos.
5. Verifiquen que `docs/index.md` se muestre correctamente como página principal.
6. Actualicen el enlace del sitio arriba en este README y entréguenlo a la cátedra antes de la fecha límite de cada entrega.

> 💡 Tip: cada vez que hagan `push` a la rama publicada, el sitio se actualiza automáticamente. No es necesario volver a configurar nada en las siguientes entregas.
