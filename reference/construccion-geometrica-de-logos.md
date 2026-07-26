# Construcción geométrica y correcciones ópticas de logos

> Cómo se **dibuja** un signo con rigor, no solo cómo se enmarca. Herencia modernista (Müller, estilo
> tipográfico internacional): la forma se construye, se justifica y se corrige a ojo. Cubre construcción
> geométrica, sistemas de proporción, correcciones ópticas, higiene de curvas y —al final— geometría
> descriptiva estricta (proyecciones). Principios, no activos ajenos.

## 0. La regla que gobierna todo: la geometría propone, el ojo dispone

Un signo se construye con geometría pero se valida **a ojo**. Lo matemáticamente exacto casi nunca se ve
correcto: el ojo no mide, interpreta. Por eso toda construcción termina en **corrección óptica** (§4).
Si tienes que elegir entre "correcto en el archivo" y "correcto a la vista", gana la vista, siempre.

## 1. Retícula de construcción y círculos guía

- **Empieza por una retícula cuadrada** (viewBox cuadrado) con una unidad base y define el signo sobre ella.
- **Círculos guía / compás y regla:** construye las curvas con circunferencias tangentes y las rectas con
  ejes de la retícula (el clásico "logo sobre grid"). No dibujes curvas "a mano" que luego no puedas justificar.
- **Un módulo, todo derivado.** Grosor de trazo, radios, aberturas y contrapunzos deben ser **fracciones del
  mismo módulo** (p. ej. trazo = 1u, radio exterior = 6u). Un signo se siente "de una pieza" cuando sus
  medidas comparten origen. Documenta la retícula: es el ADN reproducible del signo.
- **Consistencia de trazo:** mono-lineal (un solo grosor) o con contraste **deliberado y sistemático**, nunca
  accidental. Curvas y rectas del mismo peso aparente (ojo: una curva del mismo grosor *parece* más fina, §4).

## 2. Sistemas de proporción (con escepticismo sano)

Elige un sistema y sé consistente; no mezcles varios sin razón:

- **√2, √3, rectángulos raíz** — proporciones que se subdividen limpiamente; útiles para retículas y encajes.
- **Escala modular / progresión geométrica** (cada paso × una razón fija) — la forma más honesta de "armonía":
  relaciona tamaños con una razón única y verificable.
- **Fibonacci / razón áurea (φ ≈ 1,618)** — útil como *punto de partida*, pero **cuidado**: la mayoría de los
  "logos áureos" que circulan son **justificación a posteriori** (se dibujó a ojo y luego se le encajaron
  círculos de Fibonacci por marketing). No vendas misticismo áureo. Usa φ si de verdad ordena tu construcción;
  no lo pegues encima para aparentar rigor. Un agente crítico lo dice.
- **Regla práctica:** la proporción es un andamio para *empezar y verificar*, no una ley que sustituya al ojo.

## 3. Higiene de curvas (Bézier)

Un signo geométrico se arruina en los detalles de trazado:

- **Mínimos puntos de ancla**, colocados en los **extremos** de cada curva (arriba/abajo/izq/der de un círculo:
  4 puntos, no 8). Menos anclas = curvas más suaves y editables.
- **Manejadores (handles) consistentes** en dirección y tensión; para un círculo, longitud ≈ 0,552 × radio.
- **Continuidad de curva:**
  - **G1 (tangente):** las curvas se encuentran sin "esquina" — la dirección continúa.
  - **G2 (curvatura):** además, el "radio" cambia de forma continua — transiciones premium, sin destellos.
  - Una **mala tangencia** (donde una recta entra a una curva con un quiebre) es el defecto nº1 del amateur;
    se ve "roto" aunque no sepas por qué.
- **Sin superposiciones sucias:** usa espacio negativo real (`fill-rule="evenodd"`) en vez de apilar formas.

## 4. Correcciones ópticas (lo que separa a un pro)

La geometría exacta engaña al ojo. Corrige siempre:

- **Overshoot (sobrepaso):** un **círculo y un triángulo** deben **sobresalir** de la línea de caja (~1–3 %
  del alto) para *parecer* del mismo tamaño que un cuadrado o una barra recta. Sin overshoot, el círculo se ve
  pequeño y "hundido".
- **Peso aparente por forma:** a igual área, el ojo percibe distinto peso — un cuadrado pesa más que un círculo
  y que un triángulo. Ajusta tamaños para igualar **presencia**, no medidas.
- **Adelgazamiento en cruces y uniones:** donde dos trazos se juntan (una X, una Y, el vértice de una V) se
  acumula tinta y se ve **más grueso/oscuro**; adelgaza ahí (mini "ink trap") para mantener el color uniforme.
- **Horizontales más finas que verticales:** un trazo horizontal del mismo grosor *parece* más pesado; afínalo
  ligeramente para igualar el vertical (herencia tipográfica).
- **Centrado óptico, no matemático:** el centro geométrico rara vez es el centro percibido (un triángulo dentro
  de un círculo va desplazado; un signo "play" se centra a ojo, no por bounding box). Vale para logos dentro de
  contenedores/avatares.
- **Espaciado óptico** entre símbolo y wordmark, y entre letras del logotipo: se iguala **a ojo**, no por
  distancia constante (dos formas rectas necesitan más aire que una recta y una curva).

## 5. Construcción para tamaños diminutos (favicon / píxel)

- Prueba el signo a **16 px** desde el primer día; si los detalles se empastan, **simplifícalos** (versión
  reducida del símbolo, no el logo completo).
- **Alinea a la retícula de píxel** los trazos clave (grosores enteros de píxel) para que no salgan borrosos.
- Contrapunzos y aberturas mínimas: si un hueco se cierra al reducir, el signo muere. Ábrelos más de lo que
  "parece" necesario en grande.

## 6. Simetría (y cuándo romperla)

- Tipos: **reflexiva** (espejo), **rotacional** (gira n veces sobre sí), **traslacional** (repetición).
  Nombra cuál usas y por qué; da orden y memorabilidad.
- **Rompe la simetría a propósito**, no por descuido: un punto de tensión (una letra distinta, un corte)
  aporta carácter. Pero una asimetría *accidental* solo se ve como error.

## 7. Geometría descriptiva estricta (marcas dimensionales)

Cuando el signo insinúa **volumen o 3D** (monogramas isométricos, cintas plegadas, objetos imposibles), entra la
geometría descriptiva de verdad:

- **Sistemas de proyección:**
  - **Isométrica** — los tres ejes a 120°, misma escala; la más común para marcas "3D" limpias.
  - **Axonométrica (dimétrica/trimétrica)** — ejes y escalas distintas; más natural, menos rígida.
  - **Perspectiva** — con punto(s) de fuga; rara vez buena idea en un logo (no escala ni reproduce bien).
- **Construcción sobre retícula isométrica** (rombos de 30°), con las caras y aristas derivadas del mismo módulo.
- **Objetos imposibles / ambigüedad** (tipo triángulo de Penrose, cinta de Möbius): se construyen con reglas de
  proyección precisas; su gracia es geométrica, no casual.
- **Volumen y sombra construidos**, no "efecto": si hay luz, define su dirección y deriva las caras con
  coherencia proyectiva (una cara por valor), estilo modernista, sin degradados fotográficos.

**Advertencia crítica:** lo dimensional **envejece rápido y reproduce mal** (monocromo, bordado, favicon, grabado).
Úsalo solo si el volumen *es* el concepto; si no, un signo plano casi siempre gana en atemporalidad y
reproducibilidad. Ten siempre una **reducción plana** del signo dimensional.

---

### Cómo lo usa MY MULLER

- Construye el signo sobre **retícula y círculos guía**, con todas las medidas derivadas de **un módulo**.
- Usa un **sistema de proporción** como andamio, no como coartada (nada de φ decorativo).
- Cuida la **higiene Bézier** (mínimos anclas, tangencias G1/G2) y entrega SVG limpio.
- **Corrige siempre a ojo:** overshoot, uniones, horizontales, centrado y espaciado ópticos. Nómbralo al presentar.
- Prueba a **16 px** antes de enamorarte del detalle.
- Si el signo es **dimensional**, constrúyelo con proyección correcta (isométrico/axonométrico) y entrega su
  reducción plana — y pregúntate si el volumen aporta o solo estorba.
