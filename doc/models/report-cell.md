
# Report Cell

## Structure

`ReportCell`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `attributes` | [`ReportAttribute[] \| undefined`](../../doc/models/report-attribute.md) | Optional | - |
| `value` | `string \| undefined` | Optional | - |

## Example

```ts
import { ReportCell } from 'xero-accounting-apilib';

const reportCell: ReportCell = {
  attributes: [
    {
      id: 'Id4',
      value: 'Value6',
    }
  ],
  value: 'Value0',
};
```

