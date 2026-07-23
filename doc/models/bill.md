
# Bill

Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)

## Structure

`Bill`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `day` | `number \| undefined` | Optional | Day of Month (0-31) |
| `type` | [`PaymentTermTypeEnum \| undefined`](../../doc/models/payment-term-type-enum.md) | Optional | - |

## Example

```ts
import { Bill, PaymentTermTypeEnum } from 'xero-accounting-apilib';

const bill: Bill = {
  day: 214,
  type: PaymentTermTypeEnum.OFCURRENTMONTH,
};
```

