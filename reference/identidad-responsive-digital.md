# Identidad responsive (digital-first)

> Principios de una identidad pensada primero para pantalla y para adaptarse, destilados del análisis
> de manuales de marca digital-first contemporáneos. Es el **porqué** que acompaña a la plantilla
> `../templates/manual-marca-digital.md` (el **qué** a rellenar). Principios, no activos ajenos.

## 1. El logo es un sistema responsive, no un arte fijo

Igual que un layout web, la marca se adapta al espacio disponible en **niveles**, cada uno con su umbral:

1. **Lockup completo** (símbolo + wordmark) — por defecto.
2. **Lockup reducido** — para formatos extremos, con un mínimo algo menor.
3. **Solo símbolo** — cuando ni el lockup reducido cabe, se cae al símbolo aislado, con su **propio**
   tamaño mínimo.

Define el **umbral** de cada salto y el mínimo de cada nivel, en print (mm) y digital (px) por separado.
La pregunta de diseño no es "¿cuál es el logo?" sino "¿cuál es el logo **a este tamaño y en este medio**?".

## 2. Dimensionado fluido, relativo al layout

En digital, el tamaño no es un número fijo: es una **fracción del contenedor**.

- Logo como fracción del **lado corto** del layout (p. ej. vertical ~1/4, horizontal ~1/8; banners ~1/2).
- En avatares, tamaño como **% del lienzo**, medido por el **ancho** (no el alto), para que escale igual
  en cualquier resolución.
- Márgenes de colocación referidos a una medida del propio signo (p. ej. el ancho del símbolo).

## 3. Centrado óptico y conciencia del recorte

- **Centrado óptico, no matemático.** Un signo rara vez se ve centrado si lo centras por geometría; define
  un **margen inferior en %** que lo asiente ópticamente. Suele diferir entre versión cuadrada y redonda.
- **La plataforma recorta.** Muchas apps piden imagen cuadrada y la recortan a círculo. Regla: entrega el
  cuadrado ya con el margen de la versión **redonda**, para que sobreviva al recorte automático.

## 4. Variantes por plataforma / contexto de pantalla

Un mismo activo cambia según dónde vive: p. ej. en smartwatch (fondos negros) las texturas se sustituyen
por **color sólido** para ganar legibilidad. Declara las variantes por plataforma y prohíbe usarlas fuera
de su contexto. El signo se adapta al medio; su integridad, no.

## 5. Tipografía de rol bloqueado

En sistemas digitales la disciplina tipográfica se endurece: cada fuente tiene **un solo trabajo**.

- Una familia **solo para titulares** (y a veces "nunca en minúsculas, nunca como cuerpo"); otra **solo
  para cuerpo**; pesos extra reservados a dirección creativa con aprobación.
- **Cursiva solo para enfatizar** una palabra, nunca para titulares ni párrafos.
- **Disciplina hasta en el nombre:** documenta la forma correcta de escribir el nombre de la tipografía
  y los errores comunes. Un sistema fuerte controla también su metalenguaje.
- **Equivalencias por mercado:** fuentes sustitutas lo más parecidas posible para cirílico, CJK, etc.

## 6. Mismo color, distinta prominencia por contexto

Un color puede ser **acento** en comunicación de marca y a la vez **protagonista** en diseño de producto.
El rol de un color no es absoluto: depende del contexto de aplicación. Documenta el rol por contexto, no
solo el valor. (Da siempre los cuatro modelos: HEX/RGB/CMYK/Pantone.)

## 7. Guardarraíles, no leyes (pero el signo es innegociable)

Tono contemporáneo, distinto del manual-política clásico: las reglas de **dimensionado y colocación** se
enuncian como **recomendaciones** basadas en los casos más frecuentes, y pueden romperse con criterio para
servir mejor a un layout o una activación. Lo que **no** se negocia son los **usos incorrectos del signo**
(no deformar, no rotar, no recolorear, no outline, no rellenar, no sobre-brandear): ahí no hay flexibilidad.
Distingue explícitamente lo orientativo de lo inviolable.

## 8. Sistema vivo: activaciones y temporadas

La identidad no es un look congelado: define **estilos de activación** por campaña/temporada que aportan
variedad (fondos de avatar, tratamientos visuales) y **rotan en el tiempo**, pero siempre siguen la
dirección creativa anual. El sistema permite variación controlada sin perder reconocimiento.

---

### Cómo lo usa MY MULLER

- Entrega el logo como **sistema responsive** con umbrales y mínimos por nivel y por medio, no como un arte único.
- En digital, especifica tamaños y márgenes **relativos al contenedor**, no fijos.
- Resuelve avatares con **centrado óptico** y a prueba del **recorte** de la plataforma.
- Bloquea el **rol** de cada tipografía y da equivalencias por mercado.
- Separa lo **orientativo** (dimensionado, colocación) de lo **inviolable** (integridad del signo).
- Para el documento a rellenar, usa `../templates/manual-marca-digital.md`.
