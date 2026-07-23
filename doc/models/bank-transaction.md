
# Bank Transaction

Find out more here: [http://developer.xero.com/documentation/api/banktransactions/](http://developer.xero.com/documentation/api/banktransactions/)

## Structure

`BankTransaction`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bankAccount` | [`Account`](../../doc/models/account.md) | Required | Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/) |
| `bankTransactionID` | `string \| undefined` | Optional | Xero generated unique identifier for bank transaction |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `currencyRate` | `number \| undefined` | Optional | Exchange rate to base currency when money is spent or received. e.g.0.7500 Only used for bank transactions in non base currency. If this isn’t specified for non base currency accounts then either the user-defined rate (preference) or the XE.com day rate will be used. Setting currency is only supported on overpayments. |
| `date` | `string \| undefined` | Optional | Date of transaction – YYYY-MM-DD |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | Boolean to indicate if a bank transaction has an attachment<br><br>**Default**: `false` |
| `isReconciled` | `boolean \| undefined` | Optional | Boolean to show if transaction is reconciled |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[]`](../../doc/models/line-item.md) | Required | See LineItems |
| `overpaymentID` | `string \| undefined` | Optional, Read-only | Xero generated unique identifier for an Overpayment. This will be returned on BankTransactions with a Type of SPEND-OVERPAYMENT or RECEIVE-OVERPAYMENT |
| `prepaymentID` | `string \| undefined` | Optional, Read-only | Xero generated unique identifier for a Prepayment. This will be returned on BankTransactions with a Type of SPEND-PREPAYMENT or RECEIVE-PREPAYMENT |
| `reference` | `string \| undefined` | Optional | Reference for the transaction. Only supported for SPEND and RECEIVE transactions. |
| `status` | [`Status8Enum \| undefined`](../../doc/models/status-8-enum.md) | Optional | See Bank Transaction Status Codes |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `subTotal` | `number \| undefined` | Optional | Total of bank transaction excluding taxes |
| `total` | `number \| undefined` | Optional | Total of bank transaction tax inclusive |
| `totalTax` | `number \| undefined` | Optional | Total tax on bank transaction |
| `type` | [`Type5Enum`](../../doc/models/type-5-enum.md) | Required | See Bank Transaction Types |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `url` | `string \| undefined` | Optional | URL link to a source document – shown as “Go to App Name” |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import {
  AddressTypeEnum,
  BankAccountTypeEnum,
  BankTransaction,
  ClassEnum,
  CurrencyCodeEnum,
  Type5Enum,
} from 'xero-accounting-apilib';

const bankTransaction: BankTransaction = {
  bankAccount: {
    accountID: '00000000-0000-0000-0000-000000000000',
    addToWatchlist: false,
    bankAccountNumber: 'BankAccountNumber2',
    bankAccountType: BankAccountTypeEnum.BANK,
    mClass: ClassEnum.EXPENSE,
    code: '4400',
    hasAttachments: false,
    name: 'Food Sales',
    updatedDateUTC: '/Date(1573755038314)/',
  },
  lineItems: [
    {
      accountCode: 'AccountCode0',
      description: 'Description0',
      discountAmount: 58.88,
      discountRate: 40.9,
      itemCode: 'ItemCode6',
      lineItemID: '00000000-0000-0000-0000-000000000000',
      repeatingInvoiceID: '00000000-0000-0000-0000-000000000000',
    }
  ],
  type: Type5Enum.RECEIVETRANSFER,
  bankTransactionID: '00000000-0000-0000-0000-000000000000',
  contact: {
    accountNumber: 'AccountNumber2',
    accountsPayableTaxType: 'AccountsPayableTaxType2',
    accountsReceivableTaxType: 'AccountsReceivableTaxType6',
    addresses: [
      {
        addressLine1: 'AddressLine14',
        addressLine2: 'AddressLine20',
        addressLine3: 'AddressLine38',
        addressLine4: 'AddressLine46',
        addressType: AddressTypeEnum.POBOX,
      }
    ],
    attachments: [
      {
        attachmentID: '00000714-0000-0000-0000-000000000000',
        contentLength: 34,
        fileName: 'FileName6',
        includeOnline: false,
        mimeType: 'MimeType6',
      },
      {
        attachmentID: '00000714-0000-0000-0000-000000000000',
        contentLength: 34,
        fileName: 'FileName6',
        includeOnline: false,
        mimeType: 'MimeType6',
      }
    ],
  },
  currencyCode: CurrencyCodeEnum.COP,
  currencyRate: 58.46,
  date: 'Date0',
  hasAttachments: false,
  overpaymentID: '00000000-0000-0000-0000-000000000000',
  prepaymentID: '00000000-0000-0000-0000-000000000000',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

