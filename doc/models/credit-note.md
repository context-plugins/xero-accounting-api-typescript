
# Credit Note

Find out more here: [http://developer.xero.com/documentation/api/credit-notes/](http://developer.xero.com/documentation/api/credit-notes/)

## Structure

`CreditNote`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `allocations` | [`Allocation[] \| undefined`](../../doc/models/allocation.md) | Optional | See Allocations |
| `appliedAmount` | `number \| undefined` | Optional | The amount of applied to an invoice |
| `brandingThemeID` | `string \| undefined` | Optional | See BrandingThemes |
| `cISDeduction` | `number \| undefined` | Optional, Read-only | CIS deduction for UK contractors |
| `cISRate` | `number \| undefined` | Optional, Read-only | CIS Deduction rate for the organisation |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `creditNoteID` | `string \| undefined` | Optional | Xero generated unique identifier |
| `creditNoteNumber` | `string \| undefined` | Optional | ACCRECCREDIT – Unique alpha numeric code identifying credit note (when missing will auto-generate from your Organisation Invoice Settings) |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `currencyRate` | `number \| undefined` | Optional | The currency rate for a multicurrency invoice. If no rate is specified, the XE.com day rate is used |
| `date` | `string \| undefined` | Optional | The date the credit note is issued YYYY-MM-DD. If the Date element is not specified then it will default to the current date based on the timezone setting of the organisation |
| `dueDate` | `string \| undefined` | Optional | Date invoice is due – YYYY-MM-DD |
| `fullyPaidOnDate` | `string \| undefined` | Optional | Date when credit note was fully paid(UTC format) |
| `hasAttachments` | `boolean \| undefined` | Optional | boolean to indicate if a credit note has an attachment<br><br>**Default**: `false` |
| `hasErrors` | `boolean \| undefined` | Optional | A boolean to indicate if a credit note has an validation errors<br><br>**Default**: `false` |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[] \| undefined`](../../doc/models/line-item.md) | Optional | See Invoice Line Items |
| `payments` | [`Payment[] \| undefined`](../../doc/models/payment.md) | Optional | See Payments |
| `reference` | `string \| undefined` | Optional | ACCRECCREDIT only – additional reference number |
| `remainingCredit` | `number \| undefined` | Optional | The remaining credit balance on the Credit Note |
| `sentToContact` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if a credit note has been sent to a contact via  the Xero app (currently read only) |
| `status` | [`Status7Enum \| undefined`](../../doc/models/status-7-enum.md) | Optional | See Credit Note Status Codes |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `subTotal` | `number \| undefined` | Optional | The subtotal of the credit note excluding taxes |
| `total` | `number \| undefined` | Optional | The total of the Credit Note(subtotal + total tax) |
| `totalTax` | `number \| undefined` | Optional | The total tax on the credit note |
| `type` | [`Type4Enum \| undefined`](../../doc/models/type-4-enum.md) | Optional | See Credit Note Types |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of last update to the credit note |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |
| `warnings` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of warning messages from the API |

## Example

```ts
import {
  AddressTypeEnum,
  CreditNote,
  CurrencyCodeEnum,
} from 'xero-accounting-apilib';

const creditNote: CreditNote = {
  allocations: [
    {
      amount: 2.44,
      date: 'Date0',
      invoice: {
        amountCredited: 89.1,
        amountDue: 153.52,
        amountPaid: 83.36,
        attachments: [
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
        brandingThemeID: '00000b90-0000-0000-0000-000000000000',
      },
      creditNote: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 212.18,
        brandingThemeID: '00000146-0000-0000-0000-000000000000',
        cISDeduction: 239.72,
        cISRate: 189,
      },
      overpayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 99.9,
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
        currencyCode: CurrencyCodeEnum.RWF,
      },
      prepayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 126.26,
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
          },
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
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
        currencyCode: CurrencyCodeEnum.UYU,
      },
      statusAttributeString: 'StatusAttributeString2',
      validationErrors: [
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        }
      ],
    }
  ],
  appliedAmount: 2,
  brandingThemeID: '000005e2-0000-0000-0000-000000000000',
  cISDeduction: 251.52,
  cISRate: 200.8,
  hasAttachments: false,
  hasErrors: false,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

