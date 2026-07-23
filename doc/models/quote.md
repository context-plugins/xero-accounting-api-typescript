
# Quote

Find out more here: [http://developer.xero.com/documentation/api/Quotes/](http://developer.xero.com/documentation/api/Quotes/)

## Structure

`Quote`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `brandingThemeID` | `string \| undefined` | Optional | See BrandingThemes |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `currencyRate` | `number \| undefined` | Optional | The currency rate for a multicurrency quote |
| `date` | `string \| undefined` | Optional | Date quote was issued – YYYY-MM-DD. If the Date element is not specified it will default to the current date based on the timezone setting of the organisation |
| `dateString` | `string \| undefined` | Optional | Date the quote was issued (YYYY-MM-DD) |
| `expiryDate` | `string \| undefined` | Optional | Date the quote expires – YYYY-MM-DD. |
| `expiryDateString` | `string \| undefined` | Optional | Date the quote expires – YYYY-MM-DD. |
| `lineAmountTypes` | [`QuoteLineAmountTypesEnum \| undefined`](../../doc/models/quote-line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[] \| undefined`](../../doc/models/line-item.md) | Optional | See LineItems |
| `quoteID` | `string \| undefined` | Optional | QuoteID GUID is automatically generated and is returned after create or GET. |
| `quoteNumber` | `string \| undefined` | Optional | Unique alpha numeric code identifying a quote (Max Length = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `reference` | `string \| undefined` | Optional | Additional reference number<br><br>**Constraints**: *Maximum Length*: `4000` |
| `status` | [`QuoteStatusCodesEnum \| undefined`](../../doc/models/quote-status-codes-enum.md) | Optional | The status of the quote. |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `subTotal` | `number \| undefined` | Optional, Read-only | Total of quote excluding taxes. |
| `summary` | `string \| undefined` | Optional | Summary text for the quote<br><br>**Constraints**: *Maximum Length*: `3000` |
| `terms` | `string \| undefined` | Optional | Terms of the quote<br><br>**Constraints**: *Maximum Length*: `4000` |
| `title` | `string \| undefined` | Optional | Title text for the quote<br><br>**Constraints**: *Maximum Length*: `100` |
| `total` | `number \| undefined` | Optional, Read-only | Total of Quote tax inclusive (i.e. SubTotal + TotalTax). This will be ignored if it doesn’t equal the sum of the LineAmounts |
| `totalDiscount` | `number \| undefined` | Optional, Read-only | Total of discounts applied on the quote line items |
| `totalTax` | `number \| undefined` | Optional, Read-only | Total tax on quote |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import {
  AddressTypeEnum,
  CurrencyCodeEnum,
  Quote,
} from 'xero-accounting-apilib';

const quote: Quote = {
  brandingThemeID: '00002508-0000-0000-0000-000000000000',
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
  currencyCode: CurrencyCodeEnum.SBD,
  currencyRate: 127.62,
  date: 'Date8',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

