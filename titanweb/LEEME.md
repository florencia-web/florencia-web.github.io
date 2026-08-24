# Propuesta Titan Web — estado y notas

**Emitida:** 24/08/2026 · **Válida hasta:** 03/09/2026 (10 días, regla fija de Popcorn)
**Responsable:** Sol (sol@somospopcorn.com) · Florencia en copia en el mailto
**Estado:** valores cargados, logos reales, 18 secciones. Lista para publicar.

---

## 1. Valores cargados

En el objeto `PRECIOS` al final de `index.html`. Se edita el número plano y se recalcula todo solo: formato, subtotales de pago único y mensual, descuento por anticipo y correo prellenado.

| # | Ítem | Valor | Tipo |
|---|---|---|---|
| 01 | Start up de redes y pauta | $1.230.000 | único |
| 02 | Estrategia mayorista y oferta | $1.400.000 | único |
| 03 | Landing mayorista + catálogo PDF | $1.450.000 | único |
| 04 | Identidad de marca y sistema visual | $870.000 | único · opcional |
| 05 | Dirección estratégica y acompañamiento | $1.870.000 | mensual |
| 06 | Contenido (12 piezas) | $1.200.000 | mensual |
| 07 | Paid Media B2B + B2C | $890.000 **+ 15% sobre la pauta** | mensual |
| 08 | Producción audiovisual (media jornada) | $500.000 | mensual |
| 09 | Email marketing (2 newsletters) | $300.000 | mensual |

**Totales:** puesta en marcha completa **$4.950.000** · sin marca **$4.080.000** ($3.957.600 con el 3% de anticipo) · gestión mensual completa **$4.760.000/mes** · arranque recomendado 05-08 **$4.460.000/mes**. Todo + IVA.

## 2. Escenarios de pauta

| Escenario | Pauta mensual | Distribución |
|---|---|---|
| 1 · Validación | $1.200.000 | 70% Google · 30% Meta |
| 2 · **Recomendado** | $2.200.000 | 50% Google · 35% Meta · 15% retargeting |
| 3 · Escala | $3.500.000 | 45% Google · 30% Meta · 15% retargeting y recompra · 10% regional y por categoría |

El **15% de gestión no está atado a ningún escenario ni a ningún monto**: aparece como condición general (leyenda del ítem 07, fila de pauta, formas de pago y nota al pie de la sección de medios), porque todavía no sabemos cuánto van a invertir.

> **Ojo con esto:** me pediste subir el escenario base a $1.200.000, que era el valor del escenario 2. Para que la escalera siga teniendo sentido moví los tres: **1.200.000 / 2.200.000 / 3.500.000**. Si querés otro techo, se cambia en el objeto `MEDIOS` y los montos por canal se recalculan solos.

La propuesta **no promete leads ni CPL** — explica por qué (faltan cinco datos del cliente y los números de Mercado Libre que dio son incompatibles entre sí) — y en cambio define la **regla de escalado**: del 1 al 2 se pasa con 6 de cada 10 leads calificados y un costo por lead calificado que pague el margen del primer pedido; del 2 al 3, con ticket medido y segunda compra.

## 3. Formas de pago (como las pediste)

- **Puesta en marcha, 100% anticipada:** 3% de descuento sobre el valor de puesta en marcha.
- **Puesta en marcha en dos pagos:** 50% al inicio y 50% al terminar el proyecto o al mes, lo que suceda primero. Sin descuento.
- **Gestión mensual:** por mes adelantado, contrato mínimo recomendado de 6 meses.
- **Pauta:** se factura aparte, directo a las plataformas, con **15% de gestión** sobre la inversión, facturado junto al honorario mensual. Ya está sacada de todo el documento la frase "sin recargo de agencia".

## 4. Logos del logowall

Los cinco son **archivos reales**, no texto:

| Archivo | Fuente |
|---|---|
| `l-northfield.png` | northfield.edu.ar |
| `l-frambuesa.png` | frambuesadesign.com |
| `l-mercadocheque.png` | mercadocheque.com |
| `l-transpack.png` | del repo, `clientes/transpack/brand/logo/logo-full-azul.png` |
| `l-evel.png` | evel.com.ar |

Recortados, escalados y verificados sobre fondo blanco. Cada celda tiene `onerror` que cae al nombre en texto si el archivo falta.

## 5. Decisiones abiertas

- [ ] **El escenario base subió y arrastró los otros dos** (ver el aviso arriba). Confirmar los tres montos con Sol.
- [ ] **La Fase 0 la ejecuta Titan Web.** Al no haber ítem de fundación de confianza ni de deuda técnica, esos arreglos —institucional con CUIT, email corporativo, T&C, redirecciones de MercadoShops, orden de los productos sin stock— quedan como checklist priorizado dentro del ítem 05, con la salida "si prefieren que lo hagamos nosotros, se cotiza aparte". Si preferís cotizarlo, decime y lo convierto en ítem.
- [ ] **E-commerce y SEO continuo** siguen declarados como **etapa 2, a cotizar**. Pasame el valor y lo agrego como ítem mensual.
- [ ] **Email marketing (09) quedó fuera del arranque recomendado**, sumable "en cuanto la base de datos empiece a crecer". Si querés que entre desde el mes 1, se cambia la línea de recomendación.
- [x] Sección de equipo eliminada.
- [x] Caja de resumen del arranque ("Ese arranque son…") eliminada.
- [x] 15% variable desatado de los escenarios.
- [x] Responsable cambiado a Sol.

## 6. Un punto para la reunión

El ítem 06 excluye la respuesta de mensajes, y está escrito en la propuesta. **En este rubro una parte de los leads mayoristas entra por mensaje directo de Instagram**, así que ese "no incluye" tiene consecuencia comercial: si nadie de Titan Web atiende los DMs, parte de la pauta se pierde ahí. La propuesta lo plantea como definición conjunta y lo suma a "lo que necesitamos de Titan Web". Es un upsell natural si Nico dice que no tiene quién lo haga.

## 7. Sobre las imágenes

| Archivo | Origen | Nota |
|---|---|---|
| `hero-deposito.jpg` · `bazar-interior.jpg` · `importacion-cajas.jpg` · `premium-marmol.jpg` · `reposteria-mesa.jpg` | **Generadas con IA** (gpt-image-2) | Apoyo visual de contexto, sin caras. **No son fotos del depósito ni de los productos de Titan Web**, y la propuesta no las presenta como tales |
| `prod-1.jpg` … `prod-12.jpg` | **Reales**, de titanweb.com.ar | Fotos del catálogo actual (que a su vez son del proveedor) |
| `l-*.png` | Logos reales de clientes | Ver punto 4 |
| `popcorn-blanco.png` | Marca Popcorn | — |

## 8. Publicar

**GitHub Pages:** copiar `index.html` + `img/` como carpeta `titan-web/` en el repo `florencia-web.github.io` → `propuestas.somospopcorn.com/titan-web/`.
**Netlify Drop:** arrastrar la carpeta `propuesta/` completa a [app.netlify.com/drop](https://app.netlify.com/drop). Tiene que incluir `img/`.

## 9. Insumos

Auditoría del 21/08/2026 en [../auditoria/](../auditoria/): [RESUMEN-EJECUTIVO.md](../auditoria/RESUMEN-EJECUTIVO.md) · [auditoria-web.md](../auditoria/auditoria-web.md) · [auditoria-marca.md](../auditoria/auditoria-marca.md) · [analisis-mercado.md](../auditoria/analisis-mercado.md) · [inteligencia-competitiva.md](../auditoria/inteligencia-competitiva.md). Contexto en [../CLAUDE.md](../CLAUDE.md).
