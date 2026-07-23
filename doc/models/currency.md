
# Currency

Find out more here: [http://developer.xero.com/documentation/api/currencies/](http://developer.xero.com/documentation/api/currencies/)

## Structure

`Currency`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `code` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `description` | `string \| undefined` | Optional | Name of Currency |

## Example

```ts
import { Currency, CurrencyCodeEnum } from 'xero-accounting-apilib';

const currency: Currency = {
  code: CurrencyCodeEnum.BSD,
  description: 'Description6',
};
```

