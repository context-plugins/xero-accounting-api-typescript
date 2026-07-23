
# Balances

The raw AccountsReceivable(sales invoices) and AccountsPayable(bills) outstanding and overdue amounts, not converted to base currency (read only)

## Structure

`Balances`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountsPayable` | [`AccountsPayable \| undefined`](../../doc/models/accounts-payable.md) | Optional | - |
| `accountsReceivable` | [`AccountsReceivable \| undefined`](../../doc/models/accounts-receivable.md) | Optional | - |

## Example

```ts
import { Balances } from 'xero-accounting-apilib';

const balances: Balances = {
  accountsPayable: {
    outstanding: 161.92,
    overdue: 36.94,
  },
  accountsReceivable: {
    outstanding: 82,
    overdue: 213.02,
  },
};
```

