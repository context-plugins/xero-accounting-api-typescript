
# Report with Rows

## Structure

`ReportWithRows`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `reports` | [`ReportWithRow[] \| undefined`](../../doc/models/report-with-row.md) | Optional | - |

## Example

```ts
import { ReportWithRows } from 'xero-accounting-apilib';

const reportWithRows: ReportWithRows = {
  reports: [
    {
      fields: [
        {
          description: 'Description6',
          fieldID: 'FieldID8',
          value: 'Value2',
        }
      ],
      reportDate: 'ReportDate6',
      reportID: 'ReportID2',
      reportName: 'ReportName8',
      reportTitle: 'ReportTitle8',
    },
    {
      fields: [
        {
          description: 'Description6',
          fieldID: 'FieldID8',
          value: 'Value2',
        }
      ],
      reportDate: 'ReportDate6',
      reportID: 'ReportID2',
      reportName: 'ReportName8',
      reportTitle: 'ReportTitle8',
    }
  ],
};
```

