# Elemento de firma y sistema paramétrico (marca + producto)

> Cómo un **único elemento de firma**, definido por fórmulas y no por valores fijos, genera todo un
> sistema y **unifica marketing y diseño de producto**, destilado del análisis de design systems de
> marca contemporáneos y expresivos. Principios, no activos ajenos.

## 1. Un elemento de firma que genera el sistema

Las marcas más cohesivas de hoy giran en torno a **un solo motivo** —una forma, un contenedor— que nace
del logo o del nombre y se convierte en el motor de todo: contenedor de tipografía e imagen, base de la
ilustración, protagonista del motion. No es un adorno más: es **el sistema hecho forma**.

- **Deriva del significado.** El elemento sale del logo/nombre y carga un concepto (p. ej. "el que sostiene
  lo esencial"): la forma tiene una razón, no es estética arbitraria.
- **Unifica marketing y producto.** El mismo elemento vive en la campaña y en la UI: un sistema adaptativo
  que une ambos mundos en un lenguaje visual único. (Conecta con `../templates/design-tokens.md`.)

## 2. Definido por fórmulas, no por valores fijos

Lo que hace el elemento **responsive y coherente en cualquier formato** es que sus propiedades son
**ratios**, no medidas absolutas:

- **Radio de esquina = lado corto ÷ N** (p. ej. ÷6), con **mínimo y máximo por formato** para que nunca se
  vea ni demasiado cuadrado ni demasiado redondo.
- **Grosor de trazo = lado largo ÷ M** (p. ej. ÷100 normal, ÷50 pesado).
- **Padding de tipografía = % del ancho** del elemento (p. ej. 90% compacto, 70% amplio).
- **Coherencia entre instancias:** si hay varios elementos en una pieza, todos se alinean al valor
  **promedio** (ni el menor ni el mayor), para que el conjunto se sienta uno.

Documenta cada propiedad como fórmula + límites por formato; así el sistema escala solo de un banner a una valla.

## 3. El elemento tiene comportamientos, no solo forma

Un elemento de firma potente se define por lo que **hace**: contar historias, enfatizar lo importante, ser
ventana al contenido, guiar la mirada, destacar a un protagonista. Enumera sus **comportamientos** y sus
usos; es un actor con conducta, no una caja. Y ciérralo con su galería de "no hacer".

## 4. Color adaptado al contenido

Más allá de una paleta fija, el color puede **derivarse del contenido** y mantenerse sincronizado entre
producto y marketing:

- **Mundos de color** con proporciones de uso (p. ej. 60/30/10) según el tono (limpio / inmersivo / formal).
- **Color de contenido:** el color de acento se **extrae de la pieza** (del key art, por algoritmo en la UI)
  y marketing lo iguala (con cuentagotas o tomando el color dominante de la imagen). El color deja de ser
  un valor de marca para ser una **variable ligada al contenido**, común a UI y campaña.
- Mantén un verde/acento "héroe" fijo para la identidad, y un secundario que **sí** cumpla contraste WCAG.

## 5. Tipografía como expresiones nombradas

En vez de "una familia y ya", define **modos tonales con nombre** (p. ej. cotidiano, activo, narrativo),
cada uno con su **uso** y sus **métricas exactas** (peso, interlineado, tracking por nivel). La misma
familia rinde registros distintos —funcional, enérgico, editorial— sin cambiar de fuente.

## 6. Retícula derivada del aspect ratio

Método de grid portable a cualquier formato: **define la proporción del lienzo → crea un grid 1:1** (p. ej.
16×9 unidades) → **multiplica** las unidades para densificar según el formato. Márgenes iguales (p. ej. dos
unidades), espaciado uniforme, y densidad ajustada ópticamente por formato (social 30×30, valla 80×24).

## 7. Motion y sonido como extensión del mismo elemento

El sistema en movimiento **no se inventa aparte**: el propio elemento de firma anima (se contrae/expande,
su trazo se estira, brilla) y cada movimiento expresa los **principios rectores** de la marca —"todo lo que
se mueve, se mueve como la marca". Añade identidad sonora e *idents* (placas de red) por formato.

## 8. Micro-gobernanza que casi nadie escribe

Los sistemas maduros bajan al detalle operativo: formato de fechas en CTAs ("ABR 2", no "ABR 2º" ni "ABR 02"),
lockups con socios de distribución unidos por un separador vertical, badges "keyables" pre-aprobados para
garantizar legibilidad del logo sobre cualquier fondo. Lo pequeño, escrito, evita mil inconsistencias.

## 9. Todo cuelga de unos principios rectores nombrados

Cierra el círculo: un puñado de **principios con nombre** (p. ej. "hazlo diferente", "simplemente esencial",
"siempre una historia") son la fuente de la que derivan el elemento, el color, la tipografía y el motion.
Cuando dudes de una decisión, se comprueba contra los principios.

---

### Cómo lo usa MY MULLER

- Si la marca vive en muchos formatos y en producto, propón **un elemento de firma** derivado del logo que
  actúe como motor del sistema y una marketing con UI.
- Defínelo **paramétricamente** (radio, trazo, padding como fórmulas + min/max por formato; instancias al promedio).
- Dale **comportamientos** nombrados y su galería de "no hacer".
- Considera **color ligado al contenido** (mundos de color con proporciones + color extraído del key art).
- Trata la tipografía como **expresiones** con métricas, deriva la **retícula del aspect ratio**, y haz que
  el **motion** exprese los principios rectores.
