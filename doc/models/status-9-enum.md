
# Status 9 Enum

AUTHORISED or DELETED (read-only). New batch payments will have a status of AUTHORISED. It is not possible to delete batch payments via the API.

## Enumeration

`Status9Enum`

## Fields

| Name |
|  --- |
| `AUTHORISED` |
| `DELETED` |

## Example

```ts
import { Status9Enum } from 'xero-accounting-apilib';

const status9 = Status9Enum.AUTHORISED;
```

