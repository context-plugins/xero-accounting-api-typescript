
# Invoice Reminder

Find out more here: [http://developer.xero.com/documentation/api/invoice-reminders/](http://developer.xero.com/documentation/api/invoice-reminders/)

## Structure

`InvoiceReminder`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `enabled` | `boolean \| undefined` | Optional | setting for on or off |

## Example

```ts
import { InvoiceReminder } from 'xero-accounting-apilib';

const invoiceReminder: InvoiceReminder = {
  enabled: false,
};
```

