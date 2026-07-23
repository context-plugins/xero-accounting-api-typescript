
# CIS Org Setting

Find out more here: [https://developer.xero.com/documentation/api/organisation](https://developer.xero.com/documentation/api/organisation)

## Structure

`CISOrgSetting`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `cISContractorEnabled` | `boolean \| undefined` | Optional | true or false - Boolean that describes if the organisation is a CIS Contractor |
| `cISSubContractorEnabled` | `boolean \| undefined` | Optional | true or false - Boolean that describes if the organisation is a CIS SubContractor |
| `rate` | `number \| undefined` | Optional, Read-only | CIS Deduction rate for the organisation |

## Example

```ts
import { CISOrgSetting } from 'xero-accounting-apilib';

const cISOrgSetting: CISOrgSetting = {
  cISContractorEnabled: false,
  cISSubContractorEnabled: false,
  rate: 58.56,
};
```

