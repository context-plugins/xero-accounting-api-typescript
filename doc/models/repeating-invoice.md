
# Repeating Invoice

Find out more here: [http://developer.xero.com/documentation/api/repeating-invoices/](http://developer.xero.com/documentation/api/repeating-invoices/)

## Structure

`RepeatingInvoice`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `attachments` | [`Attachment[] \| undefined`](../../doc/models/attachment.md) | Optional | Displays array of attachments from the API |
| `brandingThemeID` | `string \| undefined` | Optional | See BrandingThemes |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if an invoice has an attachment<br><br>**Default**: `false` |
| `iD` | `string \| undefined` | Optional | Xero generated unique identifier for repeating invoice template |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[] \| undefined`](../../doc/models/line-item.md) | Optional | See LineItems |
| `reference` | `string \| undefined` | Optional | ACCREC only – additional reference number |
| `repeatingInvoiceID` | `string \| undefined` | Optional | Xero generated unique identifier for repeating invoice template |
| `schedule` | [`Schedule \| undefined`](../../doc/models/schedule.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/repeating-invoices/](http://developer.xero.com/documentation/api/repeating-invoices/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/repeating-invoices/](http://developer.xero.com/documentation/api/repeating-invoices/) |
| `status` | [`Status18Enum \| undefined`](../../doc/models/status-18-enum.md) | Optional | One of the following - DRAFT or AUTHORISED – See Invoice Status Codes |
| `subTotal` | `number \| undefined` | Optional | Total of invoice excluding taxes |
| `total` | `number \| undefined` | Optional | Total of Invoice tax inclusive (i.e. SubTotal + TotalTax) |
| `totalTax` | `number \| undefined` | Optional | Total tax on invoice |
| `type` | [`Type8Enum \| undefined`](../../doc/models/type-8-enum.md) | Optional | See Invoice Types |

## Example

```ts
import {
  AddressTypeEnum,
  CurrencyCodeEnum,
  RepeatingInvoice,
} from 'xero-accounting-apilib';

const repeatingInvoice: RepeatingInvoice = {
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
  brandingThemeID: '00001772-0000-0000-0000-000000000000',
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
  currencyCode: CurrencyCodeEnum.UZS,
  hasAttachments: false,
};
```

