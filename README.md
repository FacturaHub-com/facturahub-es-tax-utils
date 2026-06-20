# facturahub-es-tax-utils

**Parte del ecosistema [FacturaHub](https://facturahub.com?utm_source=github&utm_medium=referral&utm_campaign=es-tax-utils)** — facturación en España, **Verifactu**, **IVA**, **Modelo 303** y automatización fiscal con IA.

> Todas las utilidades fiscales de España en un paquete. MIT.

Reexporta, bajo espacios de nombres, las librerías individuales:

```ts
import { nif, iva, iban, facturaNumber, verifactuHash, verifactuQr, modelo303 } from 'facturahub-es-tax-utils';

nif.isValidNIF('A58818501');               // true
iva.desgloseFactura({ base: 1000, ivaTipo: 21, irpfTipo: 15 });
iban.isValidSpanishIBAN('ES9121000418450200051332');
await verifactuHash.huellaAlta(registro);
modelo303.calcularModelo303({ ventas, compras });
```

## Instalación

```bash
npm i facturahub-es-tax-utils
```

Incluye: [`nif-validator`](https://github.com/FacturaHub-com/facturahub-nif-validator), [`iva`](https://github.com/FacturaHub-com/facturahub-iva), [`iban-es`](https://github.com/FacturaHub-com/facturahub-iban-es), [`factura-number`](https://github.com/FacturaHub-com/facturahub-factura-number), [`verifactu-hash`](https://github.com/FacturaHub-com/facturahub-verifactu-hash), [`verifactu-qr`](https://github.com/FacturaHub-com/facturahub-verifactu-qr), [`modelo-303`](https://github.com/FacturaHub-com/facturahub-modelo-303).

> Nota: este meta-paquete se publica **después** de las librerías individuales (depende de ellas en npm).

---

Hecho por [**FacturaHub**](https://facturahub.com?utm_source=npm&utm_medium=referral&utm_campaign=es-tax-utils) — facturación con IA para autónomos en España. Gratis.

## Ecosistema FacturaHub
- 🌐 [FacturaHub](https://facturahub.com?utm_source=github&utm_medium=referral&utm_campaign=es-tax-utils) — la app (gratis, Verifactu incluido)
- 🔌 [facturahub-api](https://github.com/FacturaHub-com/facturahub-api) — API REST + OpenAPI 3.1
- 🤖 [facturahub-mcp](https://github.com/FacturaHub-com/facturahub-mcp) — servidor MCP (Claude, Cursor, ChatGPT)
- 🧾 [facturahub-verifactu](https://github.com/FacturaHub-com/facturahub-verifactu) — Verifactu por API
- 🧮 Librerías: nif-validator · iva · iban-es · factura-number · verifactu-qr · verifactu-hash · modelo-303
- ⚙️ Automatización: facturahub-n8n · n8n-nodes-facturahub · facturahub-woocommerce · facturahub-shopify

Temas: Verifactu · Facturación electrónica · IVA · Modelo 303 · AEAT · NIF/CIF · Autónomos · MCP · IA · España
