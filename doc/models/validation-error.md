
# Validation Error

Find out more here: [https://developer.xero.com/documentation/api/http-response-codes](https://developer.xero.com/documentation/api/http-response-codes)

## Structure

`ValidationError`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `message` | `string \| undefined` | Optional | Validation error message |

## Example

```ts
import { ValidationError } from 'xero-accounting-apilib';

const validationError: ValidationError = {
  message: 'Message4',
};
```

