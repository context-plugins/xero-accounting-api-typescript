
# Tracking Options

## Structure

`TrackingOptions`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `options` | [`TrackingOption[] \| undefined`](../../doc/models/tracking-option.md) | Optional | - |

## Example

```ts
import { Status13Enum, TrackingOptions } from 'xero-accounting-apilib';

const trackingOptions: TrackingOptions = {
  options: [
    {
      name: 'Name2',
      status: Status13Enum.ARCHIVED,
      trackingCategoryID: '00000ecc-0000-0000-0000-000000000000',
      trackingOptionID: '000009c8-0000-0000-0000-000000000000',
    },
    {
      name: 'Name2',
      status: Status13Enum.ARCHIVED,
      trackingCategoryID: '00000ecc-0000-0000-0000-000000000000',
      trackingOptionID: '000009c8-0000-0000-0000-000000000000',
    },
    {
      name: 'Name2',
      status: Status13Enum.ARCHIVED,
      trackingCategoryID: '00000ecc-0000-0000-0000-000000000000',
      trackingOptionID: '000009c8-0000-0000-0000-000000000000',
    }
  ],
};
```

