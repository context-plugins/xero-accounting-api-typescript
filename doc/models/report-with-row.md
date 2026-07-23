
# Report with Row

Find out more here: [http://developer.xero.com/documentation/api/reports/](http://developer.xero.com/documentation/api/reports/)

## Structure

`ReportWithRow`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `fields` | [`ReportFields[] \| undefined`](../../doc/models/report-fields.md) | Optional | - |
| `reportDate` | `string \| undefined` | Optional | Date of report |
| `reportID` | `string \| undefined` | Optional | Report id |
| `reportName` | `string \| undefined` | Optional | Name of the report |
| `reportTitle` | `string \| undefined` | Optional | Title of the report |
| `reportTitles` | `string[] \| undefined` | Optional | Report titles array (3 to 4 strings with the report name, orgnisation name and time frame of report) |
| `reportType` | `string \| undefined` | Optional | The type of report (BalanceSheet,ProfitLoss, etc) |
| `rows` | [`ReportRows[] \| undefined`](../../doc/models/report-rows.md) | Optional | - |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Updated Date |

## Example

```ts
import { ReportWithRow } from 'xero-accounting-apilib';

const reportWithRow: ReportWithRow = {
  fields: [
    {
      description: 'Description6',
      fieldID: 'FieldID8',
      value: 'Value2',
    }
  ],
  reportDate: 'ReportDate6',
  reportID: 'ReportID2',
  reportName: 'ReportName2',
  reportTitle: 'ReportTitle8',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

