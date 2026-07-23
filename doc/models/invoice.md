
# Invoice

Find out more here: [http://developer.xero.com/documentation/api/invoices/](http://developer.xero.com/documentation/api/invoices/)

## Structure

`Invoice`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amountCredited` | `number \| undefined` | Optional, Read-only | Sum of all credit notes, over-payments and pre-payments applied to invoice |
| `amountDue` | `number \| undefined` | Optional, Read-only | Amount remaining to be paid on invoice |
| `amountPaid` | `number \| undefined` | Optional, Read-only | Sum of payments received for invoice |
| `attachments` | [`Attachment[] \| undefined`](../../doc/models/attachment.md) | Optional | Displays array of attachments from the API |
| `brandingThemeID` | `string \| undefined` | Optional | See BrandingThemes |
| `cISDeduction` | `number \| undefined` | Optional, Read-only | CIS deduction for UK contractors |
| `cISRate` | `number \| undefined` | Optional, Read-only | CIS Deduction rate for the organisation |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `creditNotes` | [`CreditNote[] \| undefined`](../../doc/models/credit-note.md) | Optional, Read-only | Details of credit notes that have been applied to an invoice |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `currencyRate` | `number \| undefined` | Optional | The currency rate for a multicurrency invoice. If no rate is specified, the XE.com day rate is used. (max length = [18].[6]) |
| `date` | `string \| undefined` | Optional | Date invoice was issued – YYYY-MM-DD. If the Date element is not specified it will default to the current date based on the timezone setting of the organisation |
| `dueDate` | `string \| undefined` | Optional | Date invoice is due – YYYY-MM-DD |
| `expectedPaymentDate` | `string \| undefined` | Optional | Shown on sales invoices (Accounts Receivable) when this has been set |
| `fullyPaidOnDate` | `string \| undefined` | Optional, Read-only | The date the invoice was fully paid. Only returned on fully paid invoices |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if an invoice has an attachment<br><br>**Default**: `false` |
| `hasErrors` | `boolean \| undefined` | Optional | A boolean to indicate if a invoice has an validation errors<br><br>**Default**: `false` |
| `invoiceID` | `string \| undefined` | Optional | Xero generated unique identifier for invoice |
| `invoiceNumber` | `string \| undefined` | Optional | ACCREC – Unique alpha numeric code identifying invoice (when missing will auto-generate from your Organisation Invoice Settings) (max length = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `isDiscounted` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if an invoice has a discount |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[] \| undefined`](../../doc/models/line-item.md) | Optional | See LineItems |
| `overpayments` | [`Overpayment[] \| undefined`](../../doc/models/overpayment.md) | Optional, Read-only | See Overpayments |
| `payments` | [`Payment[] \| undefined`](../../doc/models/payment.md) | Optional, Read-only | See Payments |
| `plannedPaymentDate` | `string \| undefined` | Optional | Shown on bills (Accounts Payable) when this has been set |
| `prepayments` | [`Prepayment[] \| undefined`](../../doc/models/prepayment.md) | Optional, Read-only | See Prepayments |
| `reference` | `string \| undefined` | Optional | ACCREC only – additional reference number |
| `repeatingInvoiceID` | `string \| undefined` | Optional | Xero generated unique identifier for repeating invoices |
| `sentToContact` | `boolean \| undefined` | Optional | Boolean to set whether the invoice in the Xero app should be marked as “sent”. This can be set only on invoices that have been approved |
| `status` | [`Status5Enum \| undefined`](../../doc/models/status-5-enum.md) | Optional | See Invoice Status Codes |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `subTotal` | `number \| undefined` | Optional, Read-only | Total of invoice excluding taxes |
| `total` | `number \| undefined` | Optional, Read-only | Total of Invoice tax inclusive (i.e. SubTotal + TotalTax). This will be ignored if it doesn’t equal the sum of the LineAmounts |
| `totalDiscount` | `number \| undefined` | Optional, Read-only | Total of discounts applied on the invoice line items |
| `totalTax` | `number \| undefined` | Optional, Read-only | Total tax on invoice |
| `type` | [`Type3Enum \| undefined`](../../doc/models/type-3-enum.md) | Optional | See Invoice Types |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `url` | `string \| undefined` | Optional | URL link to a source document – shown as “Go to [appName]” in the Xero app |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |
| `warnings` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of warning messages from the API |

## Example

```ts
import { Invoice } from 'xero-accounting-apilib';

const invoice: Invoice = {
  amountCredited: 67.76,
  amountDue: 132.18,
  amountPaid: 62.02,
  attachments: [
    {
      attachmentID: '00000714-0000-0000-0000-000000000000',
      contentLength: 34,
      fileName: 'FileName6',
      includeOnline: false,
      mimeType: 'MimeType6',
    }
  ],
  brandingThemeID: '00000176-0000-0000-0000-000000000000',
  hasAttachments: false,
  hasErrors: false,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

