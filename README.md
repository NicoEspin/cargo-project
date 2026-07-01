# NTL Tailwind Static

Maqueta estática en `HTML + Tailwind CDN` ajustada para acercarse al Adobe XD de referencia en desktop `1366px`.

## Cómo abrirlo

Abrí `index.html` directamente en el navegador.

## Pantallas implementadas

- `index.html`
  - Busqueda principal `Move Together`
  - Estado base del card de busqueda
  - Overlay de login requerido
  - Overlay de BL erroneo
- `pages/carga-maritima.html`
  - Detalle de carga consolidado
  - Variante marítima `FCL`
  - Variante aérea `LCL`
  - Variante terrestre `LCL`
- `pages/otros-embarques.html`
  - Estado con datos
  - Estado sin datos
- `pages/estado-cuenta.html`
  - Tabla de comprobantes
  - Resumen de deuda y total adeudado
- `pages/mi-perfil.html`
  - Encabezado de empresa
  - Datos de cuenta
  - Datos fiscales
  - Datos de contacto
- `pages/estado-error.html`
  - Login requerido sobre detalle de carga
  - BL incorrecto sobre detalle de carga

## Consolidaciones explícitas

- `pages/carga-maritima.html` consolida las pantallas de carga marítima, aérea y terrestre en secciones ancladas.
- `pages/otros-embarques.html` consolida el estado con resultados y el estado vacío.
- `index.html` consolida el card de busqueda base con los overlays de login requerido y BL incorrecto.
- `pages/estado-error.html` consolida los estados de login requerido y BL incorrecto sobre detalle.

## Referencias visuales

- Archivo fuente: `design/html para desarrollar.xd`
- Capturas de referencia sin renombrar: `design/WhatsApp Image *.jpeg`

## Assets usados

- `assets/img/maersk-logo.png`
- `assets/img/carga-aerea.png`
- `assets/img/carga-maritima.png`
- `assets/img/carga-terrestre.png`

Nota: las referencias exportadas no traen nombres útiles, así que el mapeo se hizo comparando composición, navegación activa, tablas, modales y bloques de contenido.

## Pendientes respecto al XD

- Varias pantallas del XD usan iconografía específica no exportada como asset; se resolvió con SVG inline o caracteres equivalentes para no inventar imágenes.
- Algunos textos del XD aparecen como placeholders o sin dato real; se respetó la estructura visual y los valores visibles de las capturas.
- La maqueta prioriza desktop 1366px; responsive básico existe, pero no replica todas las decisiones del XD fuera de ese ancho.
- La raiz `/` quedó enfocada en el card de busqueda y sus overlays porque esa es la referencia directa del set actual.

## Navegación

- Desde `index.html#card` el buscador lleva a `pages/carga-maritima.html#maritima`.
- `index.html#login` muestra el estado de login requerido sobre la busqueda.
- `index.html#error` muestra el estado de BL erroneo sobre la busqueda.
- Las tabs superiores conectan detalle, otros embarques, estado de cuenta y perfil.
- Las variantes consolidadas usan anchors para que cada estado se pueda abrir directo.

## Verificación realizada

- Revisión manual de estructura HTML final en `index.html` y `pages/*.html`.
- Revisión de consistencia de navegación relativa entre archivos.
- Revisión de consolidaciones documentadas y accesibles por anchor.
- Revisión visual indirecta contra las capturas exportadas en `design/`.
