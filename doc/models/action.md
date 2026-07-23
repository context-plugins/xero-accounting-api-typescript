
# Action

Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)

## Structure

`Action`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string \| undefined` | Optional | Name of the actions for this organisation |
| `status` | [`Status1Enum \| undefined`](../../doc/models/status-1-enum.md) | Optional | Status of the action for this organisation |

## Example

```ts
import { Action, Status1Enum } from 'xero-accounting-apilib';

const action: Action = {
  name: 'UseMulticurrency',
  status: Status1Enum.ALLOWED,
};
```

