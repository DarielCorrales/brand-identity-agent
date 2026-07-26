# MY MULLER — Agente de Identidad de Marca

> **En honor a Jens Müller** (Koblenz, 1982), diseñador y autor de *Logo Modernism*, referente en la documentación de la identidad corporativa modernista. MY MULLER hereda esa sensibilidad: claridad sobre decoración, construcción sistemática y geométrica, y marcas pensadas para durar.

Agente especializado en **desarrollo de marca, identidad visual y sistemas de diseño**: estrategia de marca, manual de identidad, logotipos, isotipos, imagotipos e isologos, sistemas de color y tipografía, y tokens de diseño.

Una sola fuente de verdad ([`agent/core-instructions.md`](agent/core-instructions.md)) y adaptaciones listas para cada plataforma donde trabajes.

## Estructura

```
brand-identity-agent/
├── README.md                     Este archivo
├── CHANGELOG.md                  Historial de versiones
├── LICENSE                       Licencia MIT
├── .gitignore
├── agent/
│   ├── core-instructions.md      Fuente de verdad — el agente completo
│   ├── claude-project.md         Para pegar en un Proyecto de Claude
│   ├── gpt-instructions.md       Para el campo "Instructions" de un GPT (< 8000 car.)
│   └── SKILL.md                  Formato de Skill de Claude
├── reference/
│   ├── color.md                  Concepto de color ampliado
│   ├── tipografia.md             Diseño tipográfico y microajustes
│   ├── rubrica-logo.md           Rúbrica de evaluación de un logo
│   ├── sistemas-de-icono-de-marca.md   Anatomía y método de un brandbook de clase mundial
│   ├── gobernanza-y-sistema-editorial.md   Gobernanza, retícula editorial y aplicaciones
│   ├── identidad-responsive-digital.md   Principios digital-first (logo responsive, avatares, activaciones)
│   └── co-branding-y-activos-para-terceros.md   Guías de partner/licencia: co-branding, nomenclatura, activos
├── examples/
│   ├── cumbre.md                 Caso trabajado de principio a fin
│   └── cumbre-isotipo.svg        Isotipo de ejemplo (SVG editable)
└── templates/
    ├── brief-marca.md            Cuestionario de brief para arrancar un proyecto
    ├── brand-foundations.md      Bases de marca: valores, mensajería, tono de voz, personaje
    ├── logo-standards.md         Estándar de uso de un logo (para proveedores/prensa)
    ├── manual-identidad.md       Esqueleto breve de manual de identidad
    ├── manual-identidad-corporativo.md   Manual corporativo completo (6 secciones)
    ├── manual-marca-producto.md   Manual de marca de producto (activos, motion, legal)
    ├── manual-marca-digital.md   Manual digital y arquitectura (submarca, avatares, colocación)
    ├── entrega-logo.md           Checklist de entrega de un logo
    └── design-tokens.md          Puente de marca a sistema de diseño (tokens)
```

## Cómo desplegarlo en cada plataforma

**Claude (Proyecto).** Crea un Proyecto nuevo y pega el contenido de `agent/claude-project.md` en las instrucciones personalizadas. Sube las plantillas de `templates/` como conocimiento del proyecto si quieres que las use.

**Claude (Skill).** Usa `agent/SKILL.md` como base de una Skill. Mantén el bloque de metadatos (frontmatter) al inicio.

**ChatGPT (GPT personalizado).** Copia `agent/gpt-instructions.md` en el campo *Instructions*. Es una versión condensada que respeta el límite de caracteres.

**Proyectos de diseño / sistemas de diseño.** Usa las plantillas de `templates/` directamente como documentos de trabajo, y `design-tokens.md` para conectar la identidad con un sistema de diseño.

## Mantener sincronizado

`core-instructions.md` es la referencia. Cuando cambies algo importante ahí, propaga el cambio a las variantes de plataforma para que no se desincronicen.

## Licencia

MIT © 2026 Dariel Corrales. Ver [`LICENSE`](LICENSE).
