# AGENTS.md

## Objetivo del proyecto

Este proyecto es una maqueta estática basada en un archivo Adobe XD. Debe implementarse con HTML + Tailwind CSS, priorizando fidelidad visual respecto al diseño original.

## Stack permitido

- HTML
- Tailwind CSS
- JavaScript mínimo solo si es necesario para interacciones simples
- Assets locales en `/assets`

## Stack no permitido

- React
- Next.js
- Vue
- Angular
- Bootstrap
- Librerías UI externas
- Rehacer el diseño con criterio propio

## Prioridad

1. Fidelidad visual con el XD.
2. Estructura HTML clara.
3. Tailwind limpio y mantenible.
4. Responsive básico.
5. Performance y assets optimizados.

## Instrucciones para trabajar

- Usar `design/html-para-desarrollar.xd` como fuente original.
- Usar `design/references/` como referencia visual principal.
- Extraer assets del XD cuando sea posible y guardarlos en `assets/img`.
- No reemplazar assets reales por placeholders si el asset existe en el XD.
- Mantener los colores, espaciados, tamaños y jerarquía visual del diseño original.
- Si hay dudas, priorizar que se vea igual al PNG exportado.
- Documentar diferencias pendientes en README.

## Pantallas a implementar

- Home
- Error de BL o contenedor
- Login requerido / info para loguearse
- Carga aérea
- Carga terrestre
- Carga marítima
- Nueva búsqueda con BL incorrecto
- Nueva búsqueda sin autorización
- Otros embarques
- Otros embarques sin datos
- Estado de cuenta
- Mi perfil

## Criterio visual

La maqueta debe revisarse principalmente en ancho desktop de 1366px, porque las pantallas del XD están diseñadas en ese tamaño.