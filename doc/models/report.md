
# Report

Find out more here: [http://developer.xero.com/documentation/api/reports/](http://developer.xero.com/documentation/api/reports/)

## Structure

`Report`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `contacts` | [`TenNinetyNineContact[] \| undefined`](../../doc/models/ten-ninety-nine-contact.md) | Optional | - |
| `reportDate` | `string \| undefined` | Optional | Date of report |
| `reportID` | `string \| undefined` | Optional | See Prepayment Types |
| `reportName` | `string \| undefined` | Optional | See Prepayment Types |
| `reportTitle` | `string \| undefined` | Optional | See Prepayment Types |
| `reportType` | [`ReportTypeEnum \| undefined`](../../doc/models/report-type-enum.md) | Optional | See Prepayment Types |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Updated Date |

## Example

```ts
import { Report } from 'xero-accounting-apilib';

const report: Report = {
  contacts: [
    {
      box1: 165.98,
      box10: 51.22,
      box11: 1.58,
      box13: 175.52,
      box14: 72.92,
    }
  ],
  reportDate: 'ReportDate2',
  reportID: 'ReportID8',
  reportName: 'ReportName8',
  reportTitle: 'ReportTitle4',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

