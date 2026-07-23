
# History Record

Find out more here: [https://developer.xero.com/documentation/api/history-and-notes](https://developer.xero.com/documentation/api/history-and-notes)

## Structure

`HistoryRecord`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `changes` | `string \| undefined` | Optional | Name of branding theme |
| `dateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of creation date of branding theme |
| `details` | `string \| undefined` | Optional | details |
| `user` | `string \| undefined` | Optional | has a value of 0 |

## Example

```ts
import { HistoryRecord } from 'xero-accounting-apilib';

const historyRecord: HistoryRecord = {
  changes: 'Changes6',
  dateUTC: '/Date(1573755038314)/',
  details: 'Details4',
  user: 'User2',
};
```

