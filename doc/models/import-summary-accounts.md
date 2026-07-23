
# Import Summary Accounts

A summary of the accounts changes

## Structure

`ImportSummaryAccounts`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `deleted` | `number \| undefined` | Optional | The number of accounts deleted |
| `errored` | `number \| undefined` | Optional | The number of accounts that had an error |
| `locked` | `number \| undefined` | Optional | The number of locked accounts |
| `new` | `number \| undefined` | Optional | The number of new accounts created |
| `newOrUpdated` | `number \| undefined` | Optional | The number of new or updated accounts |
| `present` | `boolean \| undefined` | Optional | - |
| `system` | `number \| undefined` | Optional | The number of system accounts |
| `total` | `number \| undefined` | Optional | The total number of accounts in the org |
| `updated` | `number \| undefined` | Optional | The number of accounts updated |

## Example

```ts
import { ImportSummaryAccounts } from 'xero-accounting-apilib';

const importSummaryAccounts: ImportSummaryAccounts = {
  deleted: 1.34,
  errored: 4.08,
  locked: 62.36,
  new: 187.5,
  newOrUpdated: 191.98,
};
```

