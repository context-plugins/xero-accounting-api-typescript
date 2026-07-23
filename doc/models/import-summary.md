
# Import Summary

A summary of the import from setup endpoint

Find out more here: [https://developer.xero.com/documentation/api-guides/conversions](https://developer.xero.com/documentation/api-guides/conversions)

## Structure

`ImportSummary`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accounts` | [`ImportSummaryAccounts \| undefined`](../../doc/models/import-summary-accounts.md) | Optional | A summary of the accounts changes |
| `organisation` | [`ImportSummaryOrganisation \| undefined`](../../doc/models/import-summary-organisation.md) | Optional | - |

## Example

```ts
import { ImportSummary } from 'xero-accounting-apilib';

const importSummary: ImportSummary = {
  accounts: {
    deleted: 162.64,
    errored: 168.06,
    locked: 226.34,
    new: 232.48,
    newOrUpdated: 228,
  },
  organisation: {
    present: false,
  },
};
```

