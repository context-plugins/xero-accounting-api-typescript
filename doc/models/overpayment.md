
# Overpayment

Find out more here: [http://developer.xero.com/documentation/api/overpayments/](http://developer.xero.com/documentation/api/overpayments/)

## Structure

`Overpayment`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `allocations` | [`Allocation[] \| undefined`](../../doc/models/allocation.md) | Optional | See Allocations |
| `appliedAmount` | `number \| undefined` | Optional | The amount of applied to an invoice |
| `attachments` | [`Attachment[] \| undefined`](../../doc/models/attachment.md) | Optional | See Attachments |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `currencyRate` | `number \| undefined` | Optional | The currency rate for a multicurrency overpayment. If no rate is specified, the XE.com day rate is used |
| `date` | `string \| undefined` | Optional | The date the overpayment is created YYYY-MM-DD |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if a overpayment has an attachment<br><br>**Default**: `false` |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[] \| undefined`](../../doc/models/line-item.md) | Optional | See Overpayment Line Items |
| `overpaymentID` | `string \| undefined` | Optional | Xero generated unique identifier |
| `payments` | [`Payment[] \| undefined`](../../doc/models/payment.md) | Optional | See Payments |
| `remainingCredit` | `number \| undefined` | Optional | The remaining credit balance on the overpayment |
| `status` | [`Status3Enum \| undefined`](../../doc/models/status-3-enum.md) | Optional | See Overpayment Status Codes |
| `subTotal` | `number \| undefined` | Optional | The subtotal of the overpayment excluding taxes |
| `total` | `number \| undefined` | Optional | The total of the overpayment (subtotal + total tax) |
| `totalTax` | `number \| undefined` | Optional | The total tax on the overpayment |
| `type` | [`Type1Enum \| undefined`](../../doc/models/type-1-enum.md) | Optional | See Overpayment Types |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of last update to the overpayment |

## Example

```ts
import {
  AddressTypeEnum,
  CurrencyCodeEnum,
  Overpayment,
} from 'xero-accounting-apilib';

const overpayment: Overpayment = {
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
  currencyCode: CurrencyCodeEnum.GYD,
  hasAttachments: false,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

