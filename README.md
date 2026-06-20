# @facturahub/es-tax-utils

> Todas las utilidades fiscales de España en un paquete. MIT.

Reexporta, bajo espacios de nombres, las librerías individuales:

```ts
import { nif, iva, iban, facturaNumber, verifactuHash, verifactuQr, modelo303 } from '@facturahub/es-tax-utils';

nif.isValidNIF('A58818501');               // true
iva.desgloseFactura({ base: 1000, ivaTipo: 21, irpfTipo: 15 });
iban.isValidSpanishIBAN('ES9121000418450200051332');
await verifactuHash.huellaAlta(registro);
modelo303.calcularModelo303({ ventas, compras });
```

## Instalación

```bash
npm i @facturahub/es-tax-utils
```

Incluye: [`nif-validator`](https://github.com/FacturaHub-com/facturahub-nif-validator), [`iva`](https://github.com/FacturaHub-com/facturahub-iva), [`iban-es`](https://github.com/FacturaHub-com/facturahub-iban-es), [`factura-number`](https://github.com/FacturaHub-com/facturahub-factura-number), [`verifactu-hash`](https://github.com/FacturaHub-com/facturahub-verifactu-hash), [`verifactu-qr`](https://github.com/FacturaHub-com/facturahub-verifactu-qr), [`modelo-303`](https://github.com/FacturaHub-com/facturahub-modelo-303).

> Nota: este meta-paquete se publica **después** de las librerías individuales (depende de ellas en npm).

---

Hecho por [**FacturaHub**](https://facturahub.com?utm_source=npm&utm_medium=referral&utm_campaign=es-tax-utils) — facturación con IA para autónomos en España. Gratis.
