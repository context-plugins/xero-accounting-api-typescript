
# Online Invoices

## Structure

`OnlineInvoices`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `onlineInvoices` | [`OnlineInvoice[] \| undefined`](../../doc/models/online-invoice.md) | Optional | - |

## Example

```ts
import { OnlineInvoices } from 'xero-accounting-apilib';

const onlineInvoices: OnlineInvoices = {
  onlineInvoices: [
    {
      onlineInvoiceUrl: 'OnlineInvoiceUrl0',
    },
    {
      onlineInvoiceUrl: 'OnlineInvoiceUrl0',
    },
    {
      onlineInvoiceUrl: 'OnlineInvoiceUrl0',
    }
  ],
};
```

