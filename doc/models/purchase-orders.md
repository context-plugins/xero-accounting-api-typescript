
# Purchase Orders

## Structure

`PurchaseOrders`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `purchaseOrders` | [`PurchaseOrder[] \| undefined`](../../doc/models/purchase-order.md) | Optional | - |

## Example

```ts
import {
  AddressTypeEnum,
  CurrencyCodeEnum,
  PurchaseOrders,
} from 'xero-accounting-apilib';

const purchaseOrders: PurchaseOrders = {
  purchaseOrders: [
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
      attentionTo: 'AttentionTo4',
      brandingThemeID: '00000d68-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.TZS,
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
      attentionTo: 'AttentionTo4',
      brandingThemeID: '00000d68-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.TZS,
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
      attentionTo: 'AttentionTo4',
      brandingThemeID: '00000d68-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.TZS,
    }
  ],
};
```

