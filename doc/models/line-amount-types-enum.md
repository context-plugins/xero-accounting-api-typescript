
# Line Amount Types Enum

Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types

## Enumeration

`LineAmountTypesEnum`

## Fields

| Name |
|  --- |
| `Exclusive` |
| `Inclusive` |
| `NoTax` |

## Example

```ts
import { LineAmountTypesEnum } from 'xero-accounting-apilib';

const lineAmountTypes = LineAmountTypesEnum.Exclusive;
```

