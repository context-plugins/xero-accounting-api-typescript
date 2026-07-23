
# Invoice Reminders

## Structure

`InvoiceReminders`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `invoiceReminders` | [`InvoiceReminder[] \| undefined`](../../doc/models/invoice-reminder.md) | Optional | - |

## Example

```ts
import { InvoiceReminders } from 'xero-accounting-apilib';

const invoiceReminders: InvoiceReminders = {
  invoiceReminders: [
    {
      enabled: false,
    },
    {
      enabled: false,
    },
    {
      enabled: false,
    }
  ],
};
```

