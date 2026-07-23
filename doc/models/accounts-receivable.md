
# Accounts Receivable

## Structure

`AccountsReceivable`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `outstanding` | `number \| undefined` | Optional | - |
| `overdue` | `number \| undefined` | Optional | - |

## Example

```ts
import { AccountsReceivable } from 'xero-accounting-apilib';

const accountsReceivable: AccountsReceivable = {
  outstanding: 29.26,
  overdue: 160.28,
};
```

