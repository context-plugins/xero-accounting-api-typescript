
# Tax Rates

## Structure

`TaxRates`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `taxRates` | [`TaxRate[] \| undefined`](../../doc/models/tax-rate.md) | Optional | - |

## Example

```ts
import { TaxRates } from 'xero-accounting-apilib';

const taxRates: TaxRates = {
  taxRates: [
    {
      canApplyToAssets: false,
      canApplyToEquity: false,
      canApplyToExpenses: false,
      canApplyToLiabilities: false,
      canApplyToRevenue: false,
    },
    {
      canApplyToAssets: false,
      canApplyToEquity: false,
      canApplyToExpenses: false,
      canApplyToLiabilities: false,
      canApplyToRevenue: false,
    },
    {
      canApplyToAssets: false,
      canApplyToEquity: false,
      canApplyToExpenses: false,
      canApplyToLiabilities: false,
      canApplyToRevenue: false,
    }
  ],
};
```

