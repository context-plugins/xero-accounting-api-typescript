
# Element

Find out more here: [https://developer.xero.com/documentation/api/http-response-codes](https://developer.xero.com/documentation/api/http-response-codes)

## Structure

`Element`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bankTransactionID` | `string \| undefined` | Optional | - |
| `batchPaymentID` | `string \| undefined` | Optional | Unique ID for batch payment object with validation error |
| `contactID` | `string \| undefined` | Optional | - |
| `creditNoteID` | `string \| undefined` | Optional | - |
| `invoiceID` | `string \| undefined` | Optional | - |
| `itemID` | `string \| undefined` | Optional | - |
| `purchaseOrderID` | `string \| undefined` | Optional | - |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Array of Validation Error message |

## Example

```ts
import { Element } from 'xero-accounting-apilib';

const element: Element = {
  bankTransactionID: '0000218e-0000-0000-0000-000000000000',
  batchPaymentID: '00001a4a-0000-0000-0000-000000000000',
  contactID: '00002310-0000-0000-0000-000000000000',
  creditNoteID: '00000acc-0000-0000-0000-000000000000',
  invoiceID: '00001354-0000-0000-0000-000000000000',
};
```

