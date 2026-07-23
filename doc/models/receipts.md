
# Receipts

## Structure

`Receipts`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `receipts` | [`Receipt[] \| undefined`](../../doc/models/receipt.md) | Optional | - |

## Example

```ts
import {
  AddressTypeEnum,
  LineAmountTypesEnum,
  Receipts,
} from 'xero-accounting-apilib';

const receipts: Receipts = {
  receipts: [
    {
      attachments: [
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
      date: 'Date2',
      hasAttachments: false,
      lineAmountTypes: LineAmountTypesEnum.NoTax,
    },
    {
      attachments: [
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
      date: 'Date2',
      hasAttachments: false,
      lineAmountTypes: LineAmountTypesEnum.NoTax,
    },
    {
      attachments: [
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
      date: 'Date2',
      hasAttachments: false,
      lineAmountTypes: LineAmountTypesEnum.NoTax,
    }
  ],
};
```

