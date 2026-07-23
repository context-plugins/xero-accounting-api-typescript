
# Bank Transfer

Find out more here: [http://developer.xero.com/documentation/api/bank-transfers/](http://developer.xero.com/documentation/api/bank-transfers/)

## Structure

`BankTransfer`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount` | `number` | Required | amount of the transaction |
| `bankTransferID` | `string \| undefined` | Optional, Read-only | The identifier of the Bank Transfer |
| `createdDateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of creation date of bank transfer |
| `currencyRate` | `number \| undefined` | Optional, Read-only | The currency rate |
| `date` | `string \| undefined` | Optional | The date of the Transfer YYYY-MM-DD |
| `fromBankAccount` | [`Account`](../../doc/models/account.md) | Required | Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/) |
| `fromBankTransactionID` | `string \| undefined` | Optional, Read-only | The Bank Transaction ID for the source account |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | Boolean to indicate if a Bank Transfer has an attachment<br><br>**Default**: `false` |
| `toBankAccount` | [`Account`](../../doc/models/account.md) | Required | Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/) |
| `toBankTransactionID` | `string \| undefined` | Optional, Read-only | The Bank Transaction ID for the destination account |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import {
  BankAccountTypeEnum,
  BankTransfer,
  ClassEnum,
} from 'xero-accounting-apilib';

const bankTransfer: BankTransfer = {
  amount: 115.42,
  fromBankAccount: {
    accountID: '00000000-0000-0000-0000-000000000000',
    addToWatchlist: false,
    bankAccountNumber: 'BankAccountNumber8',
    bankAccountType: BankAccountTypeEnum.PAYPAL,
    mClass: ClassEnum.LIABILITY,
    code: '4400',
    hasAttachments: false,
    name: 'Food Sales',
    updatedDateUTC: '/Date(1573755038314)/',
  },
  toBankAccount: {
    accountID: '00000000-0000-0000-0000-000000000000',
    addToWatchlist: false,
    bankAccountNumber: 'BankAccountNumber6',
    bankAccountType: BankAccountTypeEnum.BANK,
    mClass: ClassEnum.REVENUE,
    code: '4400',
    hasAttachments: false,
    name: 'Food Sales',
    updatedDateUTC: '/Date(1573755038314)/',
  },
  bankTransferID: '000004e0-0000-0000-0000-000000000000',
  createdDateUTC: '/Date(1573755038314)/',
  currencyRate: 27.12,
  date: 'Date8',
  fromBankTransactionID: '000009e6-0000-0000-0000-000000000000',
  hasAttachments: false,
};
```

