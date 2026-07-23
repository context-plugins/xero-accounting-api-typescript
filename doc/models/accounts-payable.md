
# Accounts Payable

## Structure

`AccountsPayable`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `outstanding` | `number \| undefined` | Optional | - |
| `overdue` | `number \| undefined` | Optional | - |

## Example

```ts
import { AccountsPayable } from 'xero-accounting-apilib';

const accountsPayable: AccountsPayable = {
  outstanding: 79.98,
  overdue: 211,
};
```

