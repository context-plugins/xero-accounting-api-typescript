
# Linked Transaction

Find out more here: [http://developer.xero.com/documentation/api/linked-transactions/](http://developer.xero.com/documentation/api/linked-transactions/)

## Structure

`LinkedTransaction`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `contactID` | `string \| undefined` | Optional | Filter by the combination of ContactID and Status. Get all the linked transactions that have been assigned to a particular customer and have a particular status e.g. GET /LinkedTransactions?ContactID=4bb34b03-3378-4bb2-a0ed-6345abf3224e&Status=APPROVED. |
| `linkedTransactionID` | `string \| undefined` | Optional | The Xero identifier for an Linked Transaction e.g./LinkedTransactions/297c2dc5-cc47-4afd-8ec8-74990b8761e9 |
| `sourceLineItemID` | `string \| undefined` | Optional | The line item identifier from the source transaction. |
| `sourceTransactionID` | `string \| undefined` | Optional | Filter by the SourceTransactionID. Get all the linked transactions created from a particular ACCPAY invoice |
| `sourceTransactionTypeCode` | [`SourceTransactionTypeCodeEnum \| undefined`](../../doc/models/source-transaction-type-code-enum.md) | Optional | The Type of the source tranasction. This will be ACCPAY if the linked transaction was created from an invoice and SPEND if it was created from a bank transaction. |
| `status` | [`Status15Enum \| undefined`](../../doc/models/status-15-enum.md) | Optional | Filter by the combination of ContactID and Status. Get all the linked transactions that have been assigned to a particular customer and have a particular status e.g. GET /LinkedTransactions?ContactID=4bb34b03-3378-4bb2-a0ed-6345abf3224e&Status=APPROVED. |
| `targetLineItemID` | `string \| undefined` | Optional | The line item identifier from the target transaction. It is possible  to link multiple billable expenses to the same TargetLineItemID. |
| `targetTransactionID` | `string \| undefined` | Optional | Filter by the TargetTransactionID. Get all the linked transactions  allocated to a particular ACCREC invoice |
| `type` | [`Type7Enum \| undefined`](../../doc/models/type-7-enum.md) | Optional | This will always be BILLABLEEXPENSE. More types may be added in future. |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | The last modified date in UTC format |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import {
  LinkedTransaction,
  SourceTransactionTypeCodeEnum,
} from 'xero-accounting-apilib';

const linkedTransaction: LinkedTransaction = {
  contactID: '00000962-0000-0000-0000-000000000000',
  linkedTransactionID: '00000db0-0000-0000-0000-000000000000',
  sourceLineItemID: '000012a8-0000-0000-0000-000000000000',
  sourceTransactionID: '0000069e-0000-0000-0000-000000000000',
  sourceTransactionTypeCode: SourceTransactionTypeCodeEnum.ACCPAY,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

