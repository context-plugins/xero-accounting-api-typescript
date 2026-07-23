
# Type 5 Enum

See Bank Transaction Types

## Enumeration

`Type5Enum`

## Fields

| Name |
|  --- |
| `RECEIVE` |
| `RECEIVEOVERPAYMENT` |
| `RECEIVEPREPAYMENT` |
| `SPEND` |
| `SPENDOVERPAYMENT` |
| `SPENDPREPAYMENT` |
| `RECEIVETRANSFER` |
| `SPENDTRANSFER` |

## Example

```ts
import { Type5Enum } from 'xero-accounting-apilib';

const type5 = Type5Enum.RECEIVETRANSFER;
```

