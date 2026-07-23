
# Batch Payments

## Structure

`BatchPayments`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `batchPayments` | [`BatchPayment[] \| undefined`](../../doc/models/batch-payment.md) | Optional | - |

## Example

```ts
import {
  BankAccountTypeEnum,
  BatchPayments,
  ClassEnum,
} from 'xero-accounting-apilib';

const batchPayments: BatchPayments = {
  batchPayments: [
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 88.64,
      batchPaymentID: '00001f7a-0000-0000-0000-000000000000',
      code: 'Code2',
      date: 'Date0',
    },
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 88.64,
      batchPaymentID: '00001f7a-0000-0000-0000-000000000000',
      code: 'Code2',
      date: 'Date0',
    },
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 88.64,
      batchPaymentID: '00001f7a-0000-0000-0000-000000000000',
      code: 'Code2',
      date: 'Date0',
    }
  ],
};
```

