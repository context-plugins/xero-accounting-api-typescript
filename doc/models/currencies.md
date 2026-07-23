
# Currencies

## Structure

`Currencies`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `currencies` | [`Currency[] \| undefined`](../../doc/models/currency.md) | Optional | - |

## Example

```ts
import { Currencies, CurrencyCodeEnum } from 'xero-accounting-apilib';

const currencies: Currencies = {
  currencies: [
    {
      code: CurrencyCodeEnum.BWP,
      description: 'Description4',
    },
    {
      code: CurrencyCodeEnum.BWP,
      description: 'Description4',
    }
  ],
};
```

