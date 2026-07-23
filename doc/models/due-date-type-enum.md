
# Due Date Type Enum

the payment terms

## Enumeration

`DueDateTypeEnum`

## Fields

| Name |
|  --- |
| `DAYSAFTERBILLDATE` |
| `DAYSAFTERBILLMONTH` |
| `DAYSAFTERINVOICEDATE` |
| `DAYSAFTERINVOICEMONTH` |
| `OFCURRENTMONTH` |
| `OFFOLLOWINGMONTH` |

## Example

```ts
import { DueDateTypeEnum } from 'xero-accounting-apilib';

const dueDateType = DueDateTypeEnum.DAYSAFTERINVOICEDATE;
```

