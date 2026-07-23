
# Repeating Invoices

## Structure

`RepeatingInvoices`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `repeatingInvoices` | [`RepeatingInvoice[] \| undefined`](../../doc/models/repeating-invoice.md) | Optional | - |

## Example

```ts
import {
  AddressTypeEnum,
  CurrencyCodeEnum,
  RepeatingInvoices,
} from 'xero-accounting-apilib';

const repeatingInvoices: RepeatingInvoices = {
  repeatingInvoices: [
    {
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
      brandingThemeID: '00001f00-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.NIO,
      hasAttachments: false,
    },
    {
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
      brandingThemeID: '00001f00-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.NIO,
      hasAttachments: false,
    },
    {
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
      brandingThemeID: '00001f00-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.NIO,
      hasAttachments: false,
    }
  ],
};
```

