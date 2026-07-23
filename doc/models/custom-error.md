
# Custom Error

Find out more here: [https://developer.xero.com/documentation/api/http-response-codes](https://developer.xero.com/documentation/api/http-response-codes)

## Structure

`CustomError`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `elements` | [`Element[] \| undefined`](../../doc/models/element.md) | Optional | Array of Elements of validation Errors |
| `errorNumber` | `number \| undefined` | Optional | Exception number |
| `message` | `string \| undefined` | Optional | Exception message |
| `type` | `string \| undefined` | Optional | Exception type |

## Example

```ts
try {
  // make the API call
} catch (error) {
  if (error instanceof CustomError) {
    console.log(error.result);
  }
}
```

