# DTE JSON Schemas — El Salvador

Esquemas JSON oficiales del Ministerio de Hacienda (MH) para los Documentos Tributarios Electrónicos (DTE) del Sistema de Transmisión, con nombres de archivo uniformes para usarlos directamente en validadores y pruebas.

*Official JSON schemas from El Salvador's Ministerio de Hacienda for electronic tax documents (DTE), renamed consistently for use in validators and tests.*

## Normativa de Cumplimiento DTE v2.0

La Normativa v2.0 (25 de mayo de 2026) es obligatoria desde el **1 de diciembre de 2026**. Hasta esa fecha MH acepta también las versiones anteriores.

| Documento | `tipoDte` | Versión v2.0 | Versión anterior |
|---|---|---|---|
| Factura Electrónica | 01 | `DTE-FE-v2.json` | `DTE-FE-v1.json` |
| Comprobante de Crédito Fiscal | 03 | `DTE-CCFE-v4.json` | `DTE-CCFE-v3.json` |
| Nota de Remisión | 04 | `DTE-NRE-v4.json` | `DTE-NRE-v3.json` |
| Nota de Crédito | 05 | `DTE-NCE-v4.json` | `DTE-NCE-v3.json` |
| Nota de Débito | 06 | `DTE-NDE-v4.json` | `DTE-NDE-v3.json` |
| Comprobante de Retención | 07 | `DTE-CRE-v2.json` | `DTE-CRE-v1.json` |
| Comprobante de Liquidación | 08 | `DTE-CLE-v2.json` | `DTE-CLE-v1.json` |
| Documento Contable de Liquidación | 09 | `DTE-DCLE-v2.json` | `DTE-DCLE-v1.json` |
| Factura de Exportación | 11 | `DTE-FEXE-v3.json` | `DTE-FEXE-v1.json` |
| Factura de Sujeto Excluido | 14 | `DTE-FSEE-v2.json` | `DTE-FSEE-v1.json` |
| Comprobante de Donación | 15 | `DTE-CDE-v2.json` | `DTE-CDE-v1.json` |
| Evento de Invalidación | — | `EVT-INVALIDACION-v3.json` | `EVT-INVALIDACION-v2.json` |
| Evento de Contingencia | — | `EVT-CONTINGENCIA-v4.json` | `EVT-CONTINGENCIA-v3.json` |
| Evento de Retorno | — | `EVT-RETORNO-v1.json` | — |
| Evento de Operaciones Especiales | — | `EVT-OPERACIONES-ESPECIALES-v1.json` | — |

El Anexo V de la Normativa indica la versión 3 para el Evento de Contingencia, mientras que el paquete de esquemas de MH incluye la versión 4. Confirme con MH cuál aplica en su caso.

Los eventos de Retorno y de Operaciones Especiales requieren autorización específica de MH.

### Cuerpos de los servicios

| Archivo | Uso |
|---|---|
| `BODY_RECEPCION_DTE.json` | Cuerpo de la petición al servicio de recepción de DTE |
| `BODY_EVT_INVALIDACION.json` | Cuerpo de la petición del evento de invalidación |

## Origen

Los archivos de las versiones v2.0 son copias exactas, byte por byte, del paquete oficial `svfe-json-schemas.zip` publicado por MH en [factura.gob.sv](https://factura.gob.sv) → Información técnica y funcional → JSON Schemas. Solo cambia el nombre del archivo:

| Paquete de MH | Este repositorio |
|---|---|
| `v2/fe-f-v2.json` | `DTE-FE-v2.json` |
| `v4/fe-ccf-v4.json` | `DTE-CCFE-v4.json` |
| `v4/fe-nr-v4.json` | `DTE-NRE-v4.json` |
| `v4/fe-nc-v4.json` | `DTE-NCE-v4.json` |
| `v4/fe-nd-v4.json` | `DTE-NDE-v4.json` |
| `v2/fe-cr-v2.json` | `DTE-CRE-v2.json` |
| `v2/fe-cl-v2.json` | `DTE-CLE-v2.json` |
| `v2/fe-dcl-v2.json` | `DTE-DCLE-v2.json` |
| `v3/fe-fex-v3.json` | `DTE-FEXE-v3.json` |
| `v2/fe-fse-v2.json` | `DTE-FSEE-v2.json` |
| `v2/fe-cd-v2.json` | `DTE-CDE-v2.json` |
| `v3/invalidacion-schema-v3.json` | `EVT-INVALIDACION-v3.json` |
| `v4/contingencia-schema-v4.json` | `EVT-CONTINGENCIA-v4.json` |
| `v1/fe-eret-v1.json` | `EVT-RETORNO-v1.json` |
| `v1/fe-eop-v1.json` | `EVT-OPERACIONES-ESPECIALES-v1.json` |

Este repositorio es una ayuda comunitaria y no está afiliado a MH. Ante cualquier diferencia, prevalece lo publicado por MH.
