
# Quotes

## Structure

`Quotes`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `quotes` | [`Quote[] \| undefined`](../../doc/models/quote.md) | Optional | - |

## Example

```ts
import {
  AddressTypeEnum,
  CurrencyCodeEnum,
  Quotes,
} from 'xero-accounting-apilib';

const quotes: Quotes = {
  quotes: [
    {
      brandingThemeID: '00001082-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.USD,
      currencyRate: 75.08,
      date: 'Date4',
    },
    {
      brandingThemeID: '00001082-0000-0000-0000-000000000000',
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
      currencyCode: CurrencyCodeEnum.USD,
      currencyRate: 75.08,
      date: 'Date4',
    }
  ],
};
```

