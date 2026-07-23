
# Linked Transactions

## Structure

`LinkedTransactions`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `linkedTransactions` | [`LinkedTransaction[] \| undefined`](../../doc/models/linked-transaction.md) | Optional | - |

## Example

```ts
import {
  LinkedTransactions,
  SourceTransactionTypeCodeEnum,
} from 'xero-accounting-apilib';

const linkedTransactions: LinkedTransactions = {
  linkedTransactions: [
    {
      contactID: '00001a8c-0000-0000-0000-000000000000',
      linkedTransactionID: '00000836-0000-0000-0000-000000000000',
      sourceLineItemID: '0000017e-0000-0000-0000-000000000000',
      sourceTransactionID: '00001c84-0000-0000-0000-000000000000',
      sourceTransactionTypeCode: SourceTransactionTypeCodeEnum.ACCPAY,
    }
  ],
};
```

