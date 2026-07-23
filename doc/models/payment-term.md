
# Payment Term

Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)

## Structure

`PaymentTerm`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bills` | [`Bill \| undefined`](../../doc/models/bill.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/) |
| `sales` | [`Bill \| undefined`](../../doc/models/bill.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/) |

## Example

```ts
import { PaymentTerm, PaymentTermTypeEnum } from 'xero-accounting-apilib';

const paymentTerm: PaymentTerm = {
  bills: {
    day: 232,
    type: PaymentTermTypeEnum.DAYSAFTERBILLDATE,
  },
  sales: {
    day: 228,
    type: PaymentTermTypeEnum.DAYSAFTERBILLDATE,
  },
};
```

