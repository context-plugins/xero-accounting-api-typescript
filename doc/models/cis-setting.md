
# CIS Setting

Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)

## Structure

`CISSetting`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `cISEnabled` | `boolean \| undefined` | Optional | Boolean that describes if the contact is a CIS Subcontractor |
| `rate` | `number \| undefined` | Optional, Read-only | CIS Deduction rate for the contact if he is a subcontractor. If the contact is not CISEnabled, then the rate is not returned |

## Example

```ts
import { CISSetting } from 'xero-accounting-apilib';

const cISSetting: CISSetting = {
  cISEnabled: false,
  rate: 100.68,
};
```

