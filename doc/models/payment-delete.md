
# Payment Delete

Find out more here: [http://developer.xero.com/documentation/api/payments/](http://developer.xero.com/documentation/api/payments/)

## Structure

`PaymentDelete`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `status` | `string` | Required | The status of the payment.<br><br>**Default**: `'DELETED'` |

## Example

```ts
import { PaymentDelete } from 'xero-accounting-apilib';

const paymentDelete: PaymentDelete = {
  status: 'DELETED',
};
```

