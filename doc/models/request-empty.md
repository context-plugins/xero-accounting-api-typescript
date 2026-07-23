
# Request Empty

Find out more here: [http://developer.xero.com/documentation/api/invoice/](http://developer.xero.com/documentation/api/invoice/)

## Structure

`RequestEmpty`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `status` | `string \| undefined` | Optional | Need at least one field to create an empty JSON payload |

## Example

```ts
import { RequestEmpty } from 'xero-accounting-apilib';

const requestEmpty: RequestEmpty = {
  status: 'Status8',
};
```

