
# Tax Rate

Find out more here: [http://developer.xero.com/documentation/api/tax-rates/](http://developer.xero.com/documentation/api/tax-rates/)

## Structure

`TaxRate`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `canApplyToAssets` | `boolean \| undefined` | Optional, Read-only | Boolean to describe if tax rate can be used for asset accounts i.e.  true,false |
| `canApplyToEquity` | `boolean \| undefined` | Optional, Read-only | Boolean to describe if tax rate can be used for equity accounts i.e true,false |
| `canApplyToExpenses` | `boolean \| undefined` | Optional, Read-only | Boolean to describe if tax rate can be used for expense accounts  i.e. true,false |
| `canApplyToLiabilities` | `boolean \| undefined` | Optional, Read-only | Boolean to describe if tax rate can be used for liability accounts  i.e. true,false |
| `canApplyToRevenue` | `boolean \| undefined` | Optional, Read-only | Boolean to describe if tax rate can be used for revenue accounts i.e. true,false |
| `displayTaxRate` | `number \| undefined` | Optional, Read-only | Tax Rate (decimal to 4dp) e.g 12.5000 |
| `effectiveRate` | `number \| undefined` | Optional, Read-only | Effective Tax Rate (decimal to 4dp) e.g 12.5000 |
| `name` | `string \| undefined` | Optional | Name of tax rate |
| `reportTaxType` | [`ReportTaxTypeEnum \| undefined`](../../doc/models/report-tax-type-enum.md) | Optional | See ReportTaxTypes |
| `status` | [`Status19Enum \| undefined`](../../doc/models/status-19-enum.md) | Optional | See Status Codes |
| `taxComponents` | [`TaxComponent[] \| undefined`](../../doc/models/tax-component.md) | Optional | See TaxComponents |
| `taxType` | `string \| undefined` | Optional | The tax type |

## Example

```ts
import { TaxRate } from 'xero-accounting-apilib';

const taxRate: TaxRate = {
  canApplyToAssets: false,
  canApplyToEquity: false,
  canApplyToExpenses: false,
  canApplyToLiabilities: false,
  canApplyToRevenue: false,
};
```

