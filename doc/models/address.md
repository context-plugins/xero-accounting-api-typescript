
# Address

Find out more here: [http://developer.xero.com/documentation/api/types](http://developer.xero.com/documentation/api/types)

## Structure

`Address`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `addressLine1` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressLine2` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressLine3` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressLine4` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressType` | [`AddressTypeEnum \| undefined`](../../doc/models/address-type-enum.md) | Optional | define the type of address |
| `attentionTo` | `string \| undefined` | Optional | max length = 255<br><br>**Constraints**: *Maximum Length*: `255` |
| `city` | `string \| undefined` | Optional | max length = 255<br><br>**Constraints**: *Maximum Length*: `255` |
| `country` | `string \| undefined` | Optional | max length = 50, [A-Z], [a-z] only<br><br>**Constraints**: *Maximum Length*: `50` |
| `postalCode` | `string \| undefined` | Optional | max length = 50<br><br>**Constraints**: *Maximum Length*: `50` |
| `region` | `string \| undefined` | Optional | max length = 255<br><br>**Constraints**: *Maximum Length*: `255` |

## Example

```ts
import { Address, AddressTypeEnum } from 'xero-accounting-apilib';

const address: Address = {
  addressLine1: 'AddressLine12',
  addressLine2: 'AddressLine26',
  addressLine3: 'AddressLine32',
  addressLine4: 'AddressLine42',
  addressType: AddressTypeEnum.POBOX,
};
```

