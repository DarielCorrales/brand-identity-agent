# Caso — Planix (crítica de marca + sistema editorial + pirámide)

> Caso real trabajado con MY MULLER. Sirve de patrón de calidad **y** de honestidad: incluye lo que
> salió bien y lo que el agente **todavía no resuelve**. Fuente de contexto: workspace de Notion del
> cliente (Documento Estratégico vigente). No se reproduce material propietario; se resume el método.

## Encargo

Analizar la identidad de Planix (logo + concepto de "pirámide de madurez") y avanzar el manual de
comunicación, teniendo en cuenta el brief real del cliente.

## Qué es Planix (contexto)

E-procurement dominicano, +13 años, parte del equipo que construyó el Portal Transaccional de Compras
Públicas de RD. Arquetipo **El Gobernante** (matiz Sabio): orden, estándar, gobernanza, trazabilidad.
Sistema de marca definido: sobrio, paleta azul medianoche/berenjena/oro champán, tipografía Space
Grotesk + Inter.

## Método aplicado (bien)

1. **Primero contexto, no opinión.** Se leyó el Notion vigente y se descartó la página histórica marcada
   como superada. Sin datos reales, la crítica sería humo.
2. **Crítica que separa argumento de gusto.** Hallazgos accionados por prioridad:
   - 🔴 Tagline con faltas ("Standar & Growd") — bloqueante: una marca "Gobernante/estándar" no puede
     deletrear mal "estándar" en su firma.
   - 🟠 Orden roto de la pirámide (la cima aparecía 2.ª desde arriba).
   - 🟠 Contradicción de concepto **agua ↔ gobierno** en el isotipo.
   - 🟠 Wordmark ≠ Space Grotesk; isotipo de "nodos" genérico (falla distinción).
   - Higiene de dato: "+13 vs +15 años" sin conciliar.
3. **Sistema editorial aterrizado a la marca** (no plantilla genérica): formato, cánones de margen,
   retícula + línea base, escala tipográfica con las fuentes reales, color por rol con aviso WCAG
   (el oro champán no cumple para cuerpo pequeño).
4. **Ejecución + bucle render→crítica** (ver `planix-piramide-madurez.svg`): se rehízo la pirámide 3-2-1
   con el orden correcto; la v1 no leía como pirámide y la etiqueta "MADUREZ" salía cortada; se corrigió
   en v2 (triángulo guía + etiqueta rotada). Iterar sobre el render real, no sobre la idea.

## Autocrítica (lo que NO resuelve — honestidad)

- **La pirámide arregla el *framework*, no el *símbolo*.** Sigue montada sobre "nodos conectados", el
  cliché que se criticó en distinción. Fija el orden y el concepto de madurez; **no** resuelve que el
  isotipo se parezca a cualquier marca de datos. Ese trabajo (símbolo comprador↔proveedor distinto) queda pendiente.
- **Es un diagrama, no un logo.** Funciona en slide/manual; no es favicon ni marca reducible.
- **Los valores editoriales son defaults sensatos, no verdades.** Márgenes, escala e interlineado son un
  punto de partida razonado; **hay que probarlos en Figma con contenido real** y ajustar a ojo.
- **El SVG es material editable**, no arte final: revisar tangencias, alineación a píxel y mínimos.

## Rúbrica del entregable

| Criterio | Nota | Nota honesta |
| --- | --- | --- |
| Pertinencia (¿resuelve el encargo real?) | 🟢 | Crítica + sistema editorial atados a la marca vigente |
| Distinción del símbolo | 🔴 | No abordada aún; sigue en "nodos" |
| Reproducibilidad del sistema editorial | 🟢 | Números concretos, replicables |
| Ejecución visual | 🟡 | Pirámide correcta pero es diagrama; SVG de partida |
| Honestidad | 🟢 | Se declara lo no resuelto y los supuestos |

## Aprendizaje para el agente

- El **bucle render→crítica** (generar SVG → rasterizar → mirar → corregir) sube la ejecución de "sabe
  decir" a "sabe hacer y comprobar". Debe ser el patrón por defecto al entregar vectores.
- **Aterrizar siempre a la marca real** del cliente (fuentes, paleta, arquetipo), nunca defaults genéricos.
- Distinguir con claridad **arreglar el framework** (hecho) de **rediseñar el símbolo** (pendiente): no
  vender lo uno como lo otro.
