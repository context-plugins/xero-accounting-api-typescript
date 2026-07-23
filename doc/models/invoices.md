
# Invoices

## Structure

`Invoices`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `invoices` | [`Invoice[] \| undefined`](../../doc/models/invoice.md) | Optional | - |

## Example

```ts
import { Invoices } from 'xero-accounting-apilib';

const invoices: Invoices = {
  invoices: [
    {
      amountCredited: 149.22,
      amountDue: 213.64,
      amountPaid: 143.48,
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
      brandingThemeID: '000008b4-0000-0000-0000-000000000000',
    }
  ],
};
```

