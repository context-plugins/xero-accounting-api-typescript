
# Import Summary Object

Find out more here: [https://developer.xero.com/documentation/api-guides/conversions](https://developer.xero.com/documentation/api-guides/conversions)

## Structure

`ImportSummaryObject`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `importSummary` | [`ImportSummary \| undefined`](../../doc/models/import-summary.md) | Optional | A summary of the import from setup endpoint<br><br>Find out more here: [https://developer.xero.com/documentation/api-guides/conversions](https://developer.xero.com/documentation/api-guides/conversions)<br><br>Find out more here: [https://developer.xero.com/documentation/api-guides/conversions](https://developer.xero.com/documentation/api-guides/conversions) |

## Example

```ts
import { ImportSummaryObject } from 'xero-accounting-apilib';

const importSummaryObject: ImportSummaryObject = {
  importSummary: {
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
  },
};
```

