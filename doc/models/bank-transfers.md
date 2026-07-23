
# Bank Transfers

## Structure

`BankTransfers`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bankTransfers` | [`BankTransfer[] \| undefined`](../../doc/models/bank-transfer.md) | Optional | - |

## Example

```ts
import {
  BankAccountTypeEnum,
  BankTransfers,
  ClassEnum,
} from 'xero-accounting-apilib';

const bankTransfers: BankTransfers = {
  bankTransfers: [
    {
      amount: 103.7,
      fromBankAccount: {
        accountID: '00001364-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      toBankAccount: {
        accountID: '000014a2-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber6',
        bankAccountType: BankAccountTypeEnum.BANK,
        mClass: ClassEnum.REVENUE,
      },
      bankTransferID: '00001594-0000-0000-0000-000000000000',
      createdDateUTC: 'CreatedDateUTC6',
      currencyRate: 15.4,
      date: 'Date6',
      fromBankTransactionID: '00001682-0000-0000-0000-000000000000',
    },
    {
      amount: 103.7,
      fromBankAccount: {
        accountID: '00001364-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      toBankAccount: {
        accountID: '000014a2-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber6',
        bankAccountType: BankAccountTypeEnum.BANK,
        mClass: ClassEnum.REVENUE,
      },
      bankTransferID: '00001594-0000-0000-0000-000000000000',
      createdDateUTC: 'CreatedDateUTC6',
      currencyRate: 15.4,
      date: 'Date6',
      fromBankTransactionID: '00001682-0000-0000-0000-000000000000',
    }
  ],
};
```

