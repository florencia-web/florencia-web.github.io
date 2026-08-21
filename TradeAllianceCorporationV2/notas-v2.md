# Trade Alliance Corporation — V2 (cambio de alcance)

**Fecha:** 2026-08-21
**Base:** `Propuesta comerciale Trade alliance corporation/index.html` (v1, mayo 2026 — intacta)
**Live v1:** https://propuesta-tradealliancecorporation.somospopcorn.workers.dev/

> Documento interno. La propuesta al cliente es `index.html`.

---

## Qué cambió respecto de v1

| # | Cambio | Dónde impacta |
|---|--------|---------------|
| 1 | **Una sola opción**: queda el Escenario 03 · El ecosistema. Se eliminan Escenario 01 y 02 | Sección 03 rediseñada como propuesta única (antes eran 3 cards) · se elimina la tabla comparativa de 3 columnas |
| 2 | **Salen del presupuesto**: streaming, aftermovie, y presentación de speakers + countdown + animaciones | Se elimina el bloque de extras de la sección Inversión · pasan a un bloque explícito "Fuera de este alcance" |
| 3 | **Drone incluido** y visible | Meta del hero · facts del escenario · lista "Qué incluye" (destacado) · tabla de alcance (fila resaltada) · sección Inversión (fila "Incluido") |
| 4 | **Precio cerrado**: ARS 13.900.000 + IVA (antes Escenario 03 = 11.815.000) | Sección Inversión · resumen lateral · mailto del CTA |
| 5 | **Forma de pago**: 30% anticipo / 30% al confirmar la 2ª jornada / 40% al confirmar la última jornada. Cuotas 2 y 3 ajustadas por IPC acumulado al facturar | Bloque B de Inversión + nota de actualización |
| 6 | Nueva sección **04 · Alcance** (entregable / qué es / formato de salida) + "Fuera de este alcance" | Reemplaza la tabla comparativa |
| 7 | Se elimina el selector interactivo de escenarios + extras (y su JS). El CTA arma un mailto con el alcance fijo | Fin del archivo |
| 8 | Fecha y vigencia: agosto 2026, 10 días | Meta · footer · CTA final |

**Importes por cuota (valor a la fecha, sin IVA):** 30% = 4.170.000 · 30% = 4.170.000 · 40% = 5.560.000.

---

## Criterio estratégico detrás de los cambios

- **Una sola opción cambia la conversación.** Con tres escenarios el cliente compara precios; con uno, evalúa alcance. La sección 03 pasa a defender *qué queda instalado* en lugar de *cuánto se gasta*.
- **Lo que sale, sale declarado.** Streaming, aftermovie, speakers/countdown y activaciones quedan listados en "Fuera de este alcance" con la leyenda *propuesta aparte*. Dos motivos: evita que descubran un costo tarde (riesgo de fricción en la aprobación) y deja sembrada la segunda propuesta sin ponerle precio todavía.
- **El drone se muestra como decisión nuestra**, no como línea de presupuesto: "lo sumamos al proyecto sin costo adicional". Un extra invisible no genera valor percibido; uno declarado sí.
- **El IPC se explica, no se esconde.** La nota aclara que los importes son valores a la fecha y que el anticipo no se actualiza. Sin eso, el ajuste se lee como aumento.
- Las **activaciones (sección 06)** se dejan en la propuesta, pero rotuladas *propuesta aparte*: sirven para mostrar techo de ambición sin comprometer alcance ni precio.

---

## Pendientes

- Publicar. La v1 vive en un Worker de Cloudflare (`propuesta-tradealliancecorporation`). Definir si esta v2 reemplaza esa URL o se publica en una nueva (recomendado: URL nueva, para que la v1 siga accesible mientras se negocia).
- Armar la **propuesta de producción del día del evento** (streaming, registro, aftermovie, speakers + countdown, activaciones inmersivas, mini estudio).

---

## Iteración 2 (21/08) — tipografía y fotografía

**Cursivas: fuera de toda la propuesta.**
- Los acentos de los titulares (`.serif-italic`) pasaron de Instrument Serif *itálica* a **Inter del mismo peso, en color** (aqua sobre fondos oscuros, violeta sobre fondos claros). El titular queda de una sola tipografía y dos tonos.
- Los bloques de display (lede, pull-quote, la pregunta "¿qué hacés cuando nadie te mira?", tagline del footer) **mantienen Instrument Serif pero en romana**, sin inclinación. Así la propuesta conserva la textura editorial sin cursivas.
- Los `em` y las notas al pie (inversión, fuera de alcance) también quedaron en redonda. En el CSS no queda ni un `font-style:italic`.

**Fotografía — 3 tipos de imagen, con criterios distintos:**

1. **Trabajo real de Popcorn** (`img/yt-*.jpg`): galería de 6 producciones propias en la sección Muestra (ESAB, Losarc, pieza documental, Banco Galicia, Telecom, Expomecánica). Portadas locales bajadas de YouTube + **lightbox que reproduce el video en la propia página** (`youtube-nocookie`), con fallback a pestaña nueva si el archivo se abre como `file://`. Se eliminó el viejo bloque "Referencia 1 / Referencia 2" de Activaciones: quedaba sin contexto y ahora esos dos videos están en la galería con nombre y descripción.
2. **Referencia visual del tratamiento** (`img/ref-*.jpg` y `img/concepto-band.jpg`, `img/alcance-aerea.jpg`): 5 imágenes **generadas con IA** (gpt-image-2), sin rostros, sin texto y sin logos, tratadas oscuras para que lean como dirección de arte y no como stock. Están rotuladas en la página como *"Referencia visual del tratamiento · no son frames del proyecto"*. Van en: Concepto (local vacío después del cierre → conecta con la pregunta del eje), sección 03 (rodaje / aéreas / post) y sección 04 (banda aérea que justifica el drone).
3. **Nada de retratos de Coco ni de Matías, ni fotos que se puedan leer como Espartanos.** No tenemos material real de ellos y una foto de archivo en ese lugar sería engañosa.

**Si preferimos cero imagen generada:** reemplazar los 5 archivos `ref-*` / `*-band` por frames reales de rodajes propios (mismo nombre de archivo, sin tocar el HTML). Es el único punto que conviene decidir antes de mandarla, porque el cliente es franquiciado de Inditex y la vara visual es alta.

**Foto de fondo en el header (21/08).** El hero pasó de gradiente violeta puro a **foto de fondo + doble capa de gradiente violeta** (`img/hero-b.jpg`): set de rodaje en penumbra con la cámara y el panel de luz sobre la derecha, y el lado izquierdo en sombra para que el titular quede 100% legible. Los anillos decorativos bajaron de 0.25 a 0.13 de opacidad para no competir con la imagen. En mobile el `background-position` se corre a 72% y el velo violeta sube, así el titular manda. Alternativa descartada guardada en `img/alt/hero-auditorio.jpg` (auditorio vacío antes del evento): se eligió el set de rodaje porque la propuesta ahora vende la **serie**, no el día del evento. Para cambiarla, reemplazar las dos referencias a `img/hero-b.jpg` en el CSS de `.hero`.
