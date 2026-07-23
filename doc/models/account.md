
# Account

Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/)

## Structure

`Account`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountID` | `string \| undefined` | Optional | The Xero identifier for an account – specified as a string following  the endpoint name   e.g. /297c2dc5-cc47-4afd-8ec8-74990b8761e9 |
| `addToWatchlist` | `boolean \| undefined` | Optional | Boolean – describes whether the account is shown in the watchlist widget on the dashboard |
| `bankAccountNumber` | `string \| undefined` | Optional | For bank accounts only (Account Type BANK) |
| `bankAccountType` | [`BankAccountTypeEnum \| undefined`](../../doc/models/bank-account-type-enum.md) | Optional | For bank accounts only. See Bank Account types |
| `mClass` | [`ClassEnum \| undefined`](../../doc/models/class-enum.md) | Optional, Read-only | See Account Class Types |
| `code` | `string \| undefined` | Optional | Customer defined alpha numeric account code e.g 200 or SALES (max length = 10) |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `description` | `string \| undefined` | Optional | Description of the Account. Valid for all types of accounts except bank accounts (max length = 4000) |
| `enablePaymentsToAccount` | `boolean \| undefined` | Optional | Boolean – describes whether account can have payments applied to it |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if an account has an attachment (read only)<br><br>**Default**: `false` |
| `name` | `string \| undefined` | Optional | Name of account (max length = 150)<br><br>**Constraints**: *Maximum Length*: `150` |
| `reportingCode` | `string \| undefined` | Optional | Shown if set |
| `reportingCodeName` | `string \| undefined` | Optional, Read-only | Shown if set |
| `showInExpenseClaims` | `boolean \| undefined` | Optional | Boolean – describes whether account code is available for use with expense claims |
| `status` | [`StatusEnum \| undefined`](../../doc/models/status-enum.md) | Optional | Accounts with a status of ACTIVE can be updated to ARCHIVED. See Account Status Codes |
| `systemAccount` | [`SystemAccountEnum \| undefined`](../../doc/models/system-account-enum.md) | Optional, Read-only | If this is a system account then this element is returned. See System Account types. Note that non-system accounts may have this element set as either “” or null. |
| `taxType` | `string \| undefined` | Optional | The tax type from TaxRates |
| `type` | [`AccountTypeEnum \| undefined`](../../doc/models/account-type-enum.md) | Optional | See Account Types |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import {
  Account,
  BankAccountTypeEnum,
  ClassEnum,
} from 'xero-accounting-apilib';

const account: Account = {
  accountID: '00000000-0000-0000-0000-000000000000',
  addToWatchlist: false,
  bankAccountNumber: 'BankAccountNumber0',
  bankAccountType: BankAccountTypeEnum.PAYPAL,
  mClass: ClassEnum.ASSET,
  code: '4400',
  hasAttachments: false,
  name: 'Food Sales',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

