
# Accounts

## Structure

`Accounts`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accounts` | [`Account[] \| undefined`](../../doc/models/account.md) | Optional | - |

## Example

```ts
import {
  Accounts,
  BankAccountTypeEnum,
  ClassEnum,
} from 'xero-accounting-apilib';

const accounts: Accounts = {
  accounts: [
    {
      accountID: '000025be-0000-0000-0000-000000000000',
      addToWatchlist: false,
      bankAccountNumber: 'BankAccountNumber6',
      bankAccountType: BankAccountTypeEnum.BANK,
      mClass: ClassEnum.EQUITY,
    },
    {
      accountID: '000025be-0000-0000-0000-000000000000',
      addToWatchlist: false,
      bankAccountNumber: 'BankAccountNumber6',
      bankAccountType: BankAccountTypeEnum.BANK,
      mClass: ClassEnum.EQUITY,
    },
    {
      accountID: '000025be-0000-0000-0000-000000000000',
      addToWatchlist: false,
      bankAccountNumber: 'BankAccountNumber6',
      bankAccountType: BankAccountTypeEnum.BANK,
      mClass: ClassEnum.EQUITY,
    }
  ],
};
```

