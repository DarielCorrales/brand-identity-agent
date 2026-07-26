# De la marca al sistema de diseño (design tokens)

Los tokens traducen la identidad a decisiones reutilizables para producto y web. Usa **roles semánticos**, no solo valores sueltos: así la marca escala sin depender de HEX memorizados.

## Color
```
--color-brand-primary:   #______
--color-brand-secondary: #______
--color-bg:              #______
--color-surface:         #______
--color-text:            #______
--color-text-muted:      #______
--color-success / warning / danger: #______
```
Roles, no nombres de color: `--color-text`, no `--gris-oscuro`.

## Tipografía
```
--font-display: "______", serif/sans;
--font-body:    "______", sans-serif;

Escala (ej. 1.25 modular):
--text-xs / sm / base / lg / xl / 2xl / 3xl
```

## Espaciado
```
--space-1: 4px   --space-2: 8px   --space-3: 12px
--space-4: 16px  --space-6: 24px  --space-8: 32px
```

## Radios y sombras
```
--radius-sm / md / lg / full
--shadow-sm / md / lg
```

## Principio
Cada token debe poder rastrearse hasta una decisión de marca. Si un valor no expresa nada de la marca, probablemente sobra o debería ser un default neutro.
