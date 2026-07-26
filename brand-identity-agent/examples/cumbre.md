# Ejemplo trabajado — CUMBRE (marca ficticia)

> Caso de referencia de principio a fin. Marca **inventada** para demostrar el proceso y el nivel de detalle esperado. No es una marca real.

## 1. Brief (resumen)

- **Negocio:** CUMBRE, tostador de café de especialidad de origen único.
- **Distintivo:** trazabilidad total y tueste por lotes pequeños.
- **Público:** amantes del café, 28–45, valoran origen, calidad y honestidad.
- **Debe sentir:** confianza, altura, artesanía sin pretensión.
- **Personalidad:** honesta, elevada, cálida, precisa.
- **Evitar:** rústico saturado, clichés de saco de yute y sello vintage.
- **Uso:** bolsa (packaging), web/tienda online, Instagram.
- **Tipo de marca:** abierto → se recomienda **imagotipo** (símbolo + logotipo separables).

## 2. Estrategia

Posicionamiento: café de altura, trazable y preciso. Territorio visual: **modernismo cálido** — geometría limpia (altura, cumbre) con una paleta de tierra tostada que evita el cliché. Atributos → forma: triángulos/cimas; tono: verde profundo + acento cálido; tipografía: geométrica con un toque humano.

## 3. Dos territorios creativos

**A — "La cima" (elegido).** Isotipo geométrico de montaña/cumbre en dos tonos, con un recorte de nieve en espacio negativo. Comunica altura y precisión; escala bien y es atemporal.

**B — "El grano-curva de nivel".** Un grano de café dibujado con curvas de nivel topográficas. Más literal e ingenioso, pero más frágil a tamaño pequeño y más ligado a una moda ilustrativa. Se descarta por atemporalidad y reproducibilidad.

## 4. Núcleo — isotipo (SVG)

Ver `cumbre-isotipo.svg`. Construcción geométrica: dos triángulos (cima principal + secundaria) y un recorte de nieve.

```svg
<svg viewBox="0 0 140 120" xmlns="http://www.w3.org/2000/svg" aria-label="CUMBRE">
  <polygon points="52,26 96,98 8,98" fill="#1C3B2E"/>
  <polygon points="94,52 134,98 54,98" fill="#3E7A5A"/>
  <polygon points="52,26 63,44 41,44" fill="#F4F1EA"/>
</svg>
```

- **Versión monocroma:** los tres polígonos en un solo color (#1C3B2E), con la nieve como espacio negativo real (`fill-rule="evenodd"`).
- **Imagotipo:** isotipo a la izquierda + logotipo "CUMBRE" a la derecha, en geométrica con tracking abierto (+40) en mayúsculas para transmitir amplitud.

## 5. Sistema de color

| Rol | Nombre | HEX | Uso |
|-----|--------|-----|-----|
| Primario | Verde cumbre | #1C3B2E | Marca, texto sobre claro |
| Secundario | Verde ladera | #3E7A5A | Apoyo, ilustración |
| Acento | Tostado | #C56B3E | CTA, detalles (10 %) |
| Neutro claro | Crema | #F4F1EA | Fondos |
| Neutro oscuro | Carbón | #1A1A17 | Texto largo |

Contraste verificado: Verde cumbre sobre Crema ≈ 9:1 (AAA). Tostado se reserva para acentos, no para texto pequeño.

## 6. Sistema tipográfico

- **Display:** geométrica (p. ej. Poppins / Futura) para el logotipo y titulares — racional, limpia, "de altura".
- **Texto:** humanista legible (p. ej. Source Sans) para cuerpo.
- **Jerarquía:** título 2xl/bold, subtítulo lg/medium, cuerpo base/regular.
- **Interlineado** de cuerpo ~140 %; **kerning** afinado en el logotipo; **tracking** +40 en las mayúsculas del wordmark.

## 7. Tokens (extracto)

```
--color-brand-primary: #1C3B2E;
--color-brand-secondary: #3E7A5A;
--color-accent: #C56B3E;
--color-bg: #F4F1EA;
--color-text: #1A1A17;
--font-display: "Poppins", sans-serif;
--font-body: "Source Sans 3", sans-serif;
--radius-md: 8px;
```

## 8. Evaluación (rúbrica)

Distinción 4 · Memorabilidad 4 · Escalabilidad 5 · Atemporalidad 5 · Pertinencia 5 · Reproducibilidad 4. La nieve en negativo se simplifica a tamaño favicon; se entrega una variante sin el recorte para 16 px.
