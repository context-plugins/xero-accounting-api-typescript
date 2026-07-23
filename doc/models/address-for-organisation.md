
# Address for Organisation

Find out more here: [http://developer.xero.com/documentation/api/types](http://developer.xero.com/documentation/api/types)

## Structure

`AddressForOrganisation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `addressLine1` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressLine2` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressLine3` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressLine4` | `string \| undefined` | Optional | max length = 500<br><br>**Constraints**: *Maximum Length*: `500` |
| `addressType` | [`AddressType1Enum \| undefined`](../../doc/models/address-type-1-enum.md) | Optional | define the type of address |
| `attentionTo` | `string \| undefined` | Optional | max length = 255<br><br>**Constraints**: *Maximum Length*: `255` |
| `city` | `string \| undefined` | Optional | max length = 255<br><br>**Constraints**: *Maximum Length*: `255` |
| `country` | `string \| undefined` | Optional | max length = 50, [A-Z], [a-z] only<br><br>**Constraints**: *Maximum Length*: `50` |
| `postalCode` | `string \| undefined` | Optional | max length = 50<br><br>**Constraints**: *Maximum Length*: `50` |
| `region` | `string \| undefined` | Optional | max length = 255<br><br>**Constraints**: *Maximum Length*: `255` |

## Example

```ts
import {
  AddressForOrganisation,
  AddressType1Enum,
} from 'xero-accounting-apilib';

const addressForOrganisation: AddressForOrganisation = {
  addressLine1: 'AddressLine16',
  addressLine2: 'AddressLine28',
  addressLine3: 'AddressLine30',
  addressLine4: 'AddressLine46',
  addressType: AddressType1Enum.STREET,
};
```

