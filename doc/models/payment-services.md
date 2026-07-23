
# Payment Services

## Structure

`PaymentServices`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `paymentServices` | [`PaymentService[] \| undefined`](../../doc/models/payment-service.md) | Optional | - |

## Example

```ts
import { PaymentServices } from 'xero-accounting-apilib';

const paymentServices: PaymentServices = {
  paymentServices: [
    {
      payNowText: 'PayNowText4',
      paymentServiceID: '00000ed4-0000-0000-0000-000000000000',
      paymentServiceName: 'PaymentServiceName4',
      paymentServiceType: 'PaymentServiceType4',
      paymentServiceUrl: 'PaymentServiceUrl0',
    },
    {
      payNowText: 'PayNowText4',
      paymentServiceID: '00000ed4-0000-0000-0000-000000000000',
      paymentServiceName: 'PaymentServiceName4',
      paymentServiceType: 'PaymentServiceType4',
      paymentServiceUrl: 'PaymentServiceUrl0',
    },
    {
      payNowText: 'PayNowText4',
      paymentServiceID: '00000ed4-0000-0000-0000-000000000000',
      paymentServiceName: 'PaymentServiceName4',
      paymentServiceType: 'PaymentServiceType4',
      paymentServiceUrl: 'PaymentServiceUrl0',
    }
  ],
};
```

