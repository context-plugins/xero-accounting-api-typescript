
# CIS Settings

## Structure

`CISSettings`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `cISSettings` | [`CISSetting[] \| undefined`](../../doc/models/cis-setting.md) | Optional | - |

## Example

```ts
import { CISSettings } from 'xero-accounting-apilib';

const cISSettings: CISSettings = {
  cISSettings: [
    {
      cISEnabled: false,
      rate: 65.2,
    },
    {
      cISEnabled: false,
      rate: 65.2,
    }
  ],
};
```

