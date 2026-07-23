
# Payments

## Structure

`Payments`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `payments` | [`Payment[] \| undefined`](../../doc/models/payment.md) | Optional | - |

## Example

```ts
import {
  BankAccountTypeEnum,
  ClassEnum,
  Payments,
} from 'xero-accounting-apilib';

const payments: Payments = {
  payments: [
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 24.8,
      bankAccountNumber: 'BankAccountNumber8',
      batchPaymentID: '0000068a-0000-0000-0000-000000000000',
      code: 'Code8',
    },
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 24.8,
      bankAccountNumber: 'BankAccountNumber8',
      batchPaymentID: '0000068a-0000-0000-0000-000000000000',
      code: 'Code8',
    },
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 24.8,
      bankAccountNumber: 'BankAccountNumber8',
      batchPaymentID: '0000068a-0000-0000-0000-000000000000',
      code: 'Code8',
    }
  ],
};
```

