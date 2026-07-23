
# Payment

Find out more here: [http://developer.xero.com/documentation/api/payments/](http://developer.xero.com/documentation/api/payments/)

## Structure

`Payment`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `account` | [`Account \| undefined`](../../doc/models/account.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/) |
| `amount` | `number \| undefined` | Optional | The amount of the payment. Must be less than or equal to the outstanding amount owing on the invoice e.g. 200.00 |
| `bankAccountNumber` | `string \| undefined` | Optional | The suppliers bank account number the payment is being made to |
| `batchPaymentID` | `string \| undefined` | Optional | Present if the payment was created as part of a batch. |
| `code` | `string \| undefined` | Optional | Code of account you are using to make the payment e.g. 001 (note- not all accounts have a code value) |
| `creditNote` | [`CreditNote \| undefined`](../../doc/models/credit-note.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/credit-notes/](http://developer.xero.com/documentation/api/credit-notes/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/credit-notes/](http://developer.xero.com/documentation/api/credit-notes/) |
| `creditNoteNumber` | `string \| undefined` | Optional | Number of invoice or credit note you are applying payment to e.g. INV-4003 |
| `currencyRate` | `number \| undefined` | Optional | Exchange rate when payment is received. Only used for non base currency invoices and credit notes e.g. 0.7500 |
| `date` | `string \| undefined` | Optional | Date the payment is being made (YYYY-MM-DD) e.g. 2009-09-06 |
| `details` | `string \| undefined` | Optional | The information to appear on the supplier's bank account |
| `hasAccount` | `boolean \| undefined` | Optional | A boolean to indicate if a contact has an validation errors<br><br>**Default**: `false` |
| `hasValidationErrors` | `boolean \| undefined` | Optional | A boolean to indicate if a contact has an validation errors<br><br>**Default**: `false` |
| `invoice` | [`Invoice \| undefined`](../../doc/models/invoice.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/invoices/](http://developer.xero.com/documentation/api/invoices/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/invoices/](http://developer.xero.com/documentation/api/invoices/) |
| `invoiceNumber` | `string \| undefined` | Optional | Number of invoice or credit note you are applying payment to e.g.INV-4003 |
| `isReconciled` | `boolean \| undefined` | Optional | An optional parameter for the payment. A boolean indicating whether you would like the payment to be created as reconciled when using PUT, or whether a payment has been reconciled when using GET |
| `overpayment` | [`Overpayment \| undefined`](../../doc/models/overpayment.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/overpayments/](http://developer.xero.com/documentation/api/overpayments/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/overpayments/](http://developer.xero.com/documentation/api/overpayments/) |
| `particulars` | `string \| undefined` | Optional | The suppliers bank account number the payment is being made to |
| `paymentID` | `string \| undefined` | Optional | The Xero identifier for an Payment e.g. 297c2dc5-cc47-4afd-8ec8-74990b8761e9 |
| `paymentType` | [`PaymentTypeEnum \| undefined`](../../doc/models/payment-type-enum.md) | Optional, Read-only | See Payment Types. |
| `prepayment` | [`Prepayment \| undefined`](../../doc/models/prepayment.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/prepayments/](http://developer.xero.com/documentation/api/prepayments/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/prepayments/](http://developer.xero.com/documentation/api/prepayments/) |
| `reference` | `string \| undefined` | Optional | An optional description for the payment e.g. Direct Debit |
| `status` | [`Status6Enum \| undefined`](../../doc/models/status-6-enum.md) | Optional | The status of the payment. |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of last update to the payment |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import {
  BankAccountTypeEnum,
  ClassEnum,
  Payment,
} from 'xero-accounting-apilib';

const payment: Payment = {
  account: {
    accountID: '00002304-0000-0000-0000-000000000000',
    addToWatchlist: false,
    bankAccountNumber: 'BankAccountNumber8',
    bankAccountType: BankAccountTypeEnum.PAYPAL,
    mClass: ClassEnum.LIABILITY,
  },
  amount: 254.28,
  bankAccountNumber: 'BankAccountNumber6',
  batchPaymentID: '00000000-0000-0000-0000-000000000000',
  code: 'Code6',
  hasAccount: false,
  hasValidationErrors: false,
  paymentID: '00000000-0000-0000-0000-000000000000',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

