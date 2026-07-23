
# History Records

## Structure

`HistoryRecords`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `historyRecords` | [`HistoryRecord[] \| undefined`](../../doc/models/history-record.md) | Optional | - |

## Example

```ts
import { HistoryRecords } from 'xero-accounting-apilib';

const historyRecords: HistoryRecords = {
  historyRecords: [
    {
      changes: 'Changes6',
      dateUTC: 'DateUTC8',
      details: 'Details4',
      user: 'User2',
    },
    {
      changes: 'Changes6',
      dateUTC: 'DateUTC8',
      details: 'Details4',
      user: 'User2',
    },
    {
      changes: 'Changes6',
      dateUTC: 'DateUTC8',
      details: 'Details4',
      user: 'User2',
    }
  ],
};
```

