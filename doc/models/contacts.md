
# Contacts

## Structure

`Contacts`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `contacts` | [`Contact[] \| undefined`](../../doc/models/contact.md) | Optional | - |

## Example

```ts
import { AddressTypeEnum, Contacts } from 'xero-accounting-apilib';

const contacts: Contacts = {
  contacts: [
    {
      accountNumber: 'AccountNumber6',
      accountsPayableTaxType: 'AccountsPayableTaxType6',
      accountsReceivableTaxType: 'AccountsReceivableTaxType2',
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
    }
  ],
};
```

