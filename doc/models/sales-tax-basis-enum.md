
# Sales Tax Basis Enum

The accounting basis used for tax returns. See Sales Tax Basis

## Enumeration

`SalesTaxBasisEnum`

## Fields

| Name |
|  --- |
| `PAYMENTS` |
| `INVOICE` |
| `NONE` |
| `CASH` |
| `ACCRUAL` |
| `FLATRATECASH` |
| `FLATRATEACCRUAL` |
| `ACCRUALS` |

## Example

```ts
import { SalesTaxBasisEnum } from 'xero-accounting-apilib';

const salesTaxBasis = SalesTaxBasisEnum.NONE;
```

