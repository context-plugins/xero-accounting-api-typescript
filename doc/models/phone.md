
# Phone

Find out more here: [http://developer.xero.com/documentation/api/types](http://developer.xero.com/documentation/api/types)

## Structure

`Phone`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `phoneAreaCode` | `string \| undefined` | Optional | max length = 10<br><br>**Constraints**: *Maximum Length*: `10` |
| `phoneCountryCode` | `string \| undefined` | Optional | max length = 20<br><br>**Constraints**: *Maximum Length*: `20` |
| `phoneNumber` | `string \| undefined` | Optional | max length = 50<br><br>**Constraints**: *Maximum Length*: `50` |
| `phoneType` | [`PhoneTypeEnum \| undefined`](../../doc/models/phone-type-enum.md) | Optional | - |

## Example

```ts
import { Phone, PhoneTypeEnum } from 'xero-accounting-apilib';

const phone: Phone = {
  phoneAreaCode: 'PhoneAreaCode8',
  phoneCountryCode: 'PhoneCountryCode6',
  phoneNumber: 'PhoneNumber2',
  phoneType: PhoneTypeEnum.DEFAULT,
};
```

