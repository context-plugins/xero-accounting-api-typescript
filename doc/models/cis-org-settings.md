
# CIS Org Settings

## Structure

`CISOrgSettings`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `cISSettings` | [`CISOrgSetting[] \| undefined`](../../doc/models/cis-org-setting.md) | Optional | - |

## Example

```ts
import { CISOrgSettings } from 'xero-accounting-apilib';

const cISOrgSettings: CISOrgSettings = {
  cISSettings: [
    {
      cISContractorEnabled: false,
      cISSubContractorEnabled: false,
      rate: 65.2,
    },
    {
      cISContractorEnabled: false,
      cISSubContractorEnabled: false,
      rate: 65.2,
    }
  ],
};
```

