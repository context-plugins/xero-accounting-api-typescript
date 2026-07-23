
# Source Transaction Type Code Enum

The Type of the source tranasction. This will be ACCPAY if the linked transaction was created from an invoice and SPEND if it was created from a bank transaction.

## Enumeration

`SourceTransactionTypeCodeEnum`

## Fields

| Name |
|  --- |
| `ACCPAY` |
| `SPEND` |

## Example

```ts
import { SourceTransactionTypeCodeEnum } from 'xero-accounting-apilib';

const sourceTransactionTypeCode = SourceTransactionTypeCodeEnum.ACCPAY;
```

