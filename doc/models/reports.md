
# Reports

## Structure

`Reports`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `reports` | [`Report[] \| undefined`](../../doc/models/report.md) | Optional | - |

## Example

```ts
import { Reports } from 'xero-accounting-apilib';

const reports: Reports = {
  reports: [
    {
      contacts: [
        {
          box1: 165.98,
          box10: 51.22,
          box11: 1.58,
          box13: 175.52,
          box14: 72.92,
        },
        {
          box1: 165.98,
          box10: 51.22,
          box11: 1.58,
          box13: 175.52,
          box14: 72.92,
        },
        {
          box1: 165.98,
          box10: 51.22,
          box11: 1.58,
          box13: 175.52,
          box14: 72.92,
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

