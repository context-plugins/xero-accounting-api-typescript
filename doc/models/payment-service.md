
# Payment Service

Find out more here: [http://developer.xero.com/documentation/api/branding-themes/](http://developer.xero.com/documentation/api/branding-themes/)

## Structure

`PaymentService`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `payNowText` | `string \| undefined` | Optional | The text displayed on the Pay Now button in Xero Online Invoicing. If this is not set it will default to Pay by credit card |
| `paymentServiceID` | `string \| undefined` | Optional | Xero identifier |
| `paymentServiceName` | `string \| undefined` | Optional | Name of payment service |
| `paymentServiceType` | `string \| undefined` | Optional | This will always be CUSTOM for payment services created via the API. |
| `paymentServiceUrl` | `string \| undefined` | Optional | The custom payment URL |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import { PaymentService } from 'xero-accounting-apilib';

const paymentService: PaymentService = {
  payNowText: 'PayNowText0',
  paymentServiceID: '00000e6a-0000-0000-0000-000000000000',
  paymentServiceName: 'PaymentServiceName0',
  paymentServiceType: 'PaymentServiceType0',
  paymentServiceUrl: 'PaymentServiceUrl6',
};
```

