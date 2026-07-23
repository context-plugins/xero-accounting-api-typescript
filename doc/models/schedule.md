
# Schedule

Find out more here: [http://developer.xero.com/documentation/api/repeating-invoices/](http://developer.xero.com/documentation/api/repeating-invoices/)

## Structure

`Schedule`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `dueDate` | `number \| undefined` | Optional | Integer used with due date type e.g 20 (of following month), 31 (of current month) |
| `dueDateType` | [`DueDateTypeEnum \| undefined`](../../doc/models/due-date-type-enum.md) | Optional | the payment terms |
| `endDate` | `string \| undefined` | Optional | Invoice end date – only returned if the template has an end date set |
| `nextScheduledDate` | `string \| undefined` | Optional | The calendar date of the next invoice in the schedule to be generated |
| `period` | `number \| undefined` | Optional | Integer used with the unit e.g. 1 (every 1 week), 2 (every 2 months) |
| `startDate` | `string \| undefined` | Optional | Date the first invoice of the current version of the repeating schedule was generated (changes when repeating invoice is edited) |
| `unit` | [`UnitEnum \| undefined`](../../doc/models/unit-enum.md) | Optional | One of the following - WEEKLY or MONTHLY |

## Example

```ts
import { DueDateTypeEnum, Schedule } from 'xero-accounting-apilib';

const schedule: Schedule = {
  dueDate: 20,
  dueDateType: DueDateTypeEnum.DAYSAFTERINVOICEDATE,
  endDate: 'EndDate6',
  nextScheduledDate: 'NextScheduledDate4',
  period: 64,
};
```

