
# Tax Component

Find out more here: [http://developer.xero.com/documentation/api/tax-rates/](http://developer.xero.com/documentation/api/tax-rates/)

## Structure

`TaxComponent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `isCompound` | `boolean \| undefined` | Optional | Boolean to describe if Tax rate is compounded. |
| `isNonRecoverable` | `boolean \| undefined` | Optional | Boolean to describe if tax rate is non-recoverable. Non-recoverable rates are only applicable to Canadian organisations |
| `name` | `string \| undefined` | Optional | Name of Tax Component |
| `rate` | `number \| undefined` | Optional | Tax Rate (up to 4dp) |

## Example

```ts
import { TaxComponent } from 'xero-accounting-apilib';

const taxComponent: TaxComponent = {
  isCompound: false,
  isNonRecoverable: false,
  name: 'Name6',
  rate: 30.52,
};
```

