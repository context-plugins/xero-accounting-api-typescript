
# Report Row

## Structure

`ReportRow`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `cells` | [`ReportCell[] \| undefined`](../../doc/models/report-cell.md) | Optional | - |
| `rowType` | [`RowTypeEnum \| undefined`](../../doc/models/row-type-enum.md) | Optional | - |
| `title` | `string \| undefined` | Optional | - |

## Example

```ts
import { ReportRow, RowTypeEnum } from 'xero-accounting-apilib';

const reportRow: ReportRow = {
  cells: [
    {
      attributes: [
        {
          id: 'Id4',
          value: 'Value6',
        },
        {
          id: 'Id4',
          value: 'Value6',
        },
        {
          id: 'Id4',
          value: 'Value6',
        }
      ],
      value: 'Value0',
    },
    {
      attributes: [
        {
          id: 'Id4',
          value: 'Value6',
        },
        {
          id: 'Id4',
          value: 'Value6',
        },
        {
          id: 'Id4',
          value: 'Value6',
        }
      ],
      value: 'Value0',
    }
  ],
  rowType: RowTypeEnum.Row,
  title: 'Title4',
};
```

