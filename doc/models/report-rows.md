
# Report Rows

## Structure

`ReportRows`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `cells` | [`ReportCell[] \| undefined`](../../doc/models/report-cell.md) | Optional | - |
| `rowType` | [`RowTypeEnum \| undefined`](../../doc/models/row-type-enum.md) | Optional | - |
| `rows` | [`ReportRow[] \| undefined`](../../doc/models/report-row.md) | Optional | - |
| `title` | `string \| undefined` | Optional | - |

## Example

```ts
import { ReportRows, RowTypeEnum } from 'xero-accounting-apilib';

const reportRows: ReportRows = {
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
  rows: [
    {
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
    }
  ],
  title: 'Title6',
};
```

