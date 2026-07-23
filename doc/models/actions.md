
# Actions

## Structure

`Actions`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `actions` | [`Action[] \| undefined`](../../doc/models/action.md) | Optional | - |

## Example

```ts
import { Actions, Status1Enum } from 'xero-accounting-apilib';

const actions: Actions = {
  actions: [
    {
      name: 'Name4',
      status: Status1Enum.ALLOWED,
    },
    {
      name: 'Name4',
      status: Status1Enum.ALLOWED,
    },
    {
      name: 'Name4',
      status: Status1Enum.ALLOWED,
    }
  ],
};
```

