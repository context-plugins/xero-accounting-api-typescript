
# Tracking Category

Find out more here: [http://developer.xero.com/documentation/api/tracking-categories/](http://developer.xero.com/documentation/api/tracking-categories/)

## Structure

`TrackingCategory`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string \| undefined` | Optional | The name of the tracking category e.g. Department, Region (max length = 100)<br><br>**Constraints**: *Maximum Length*: `100` |
| `option` | `string \| undefined` | Optional | The option name of the tracking option e.g. East, West (max length = 100)<br><br>**Constraints**: *Maximum Length*: `100` |
| `options` | [`TrackingOption[] \| undefined`](../../doc/models/tracking-option.md) | Optional | See Tracking Options |
| `status` | [`Status14Enum \| undefined`](../../doc/models/status-14-enum.md) | Optional | The status of a tracking category |
| `trackingCategoryID` | `string \| undefined` | Optional | The Xero identifier for a tracking category e.g. 297c2dc5-cc47-4afd-8ec8-74990b8761e9 |
| `trackingOptionID` | `string \| undefined` | Optional | The Xero identifier for a tracking option e.g. dc54c220-0140-495a-b925-3246adc0075f |

## Example

```ts
import {
  Status13Enum,
  Status14Enum,
  TrackingCategory,
} from 'xero-accounting-apilib';

const trackingCategory: TrackingCategory = {
  name: 'Name4',
  option: 'Option4',
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
    }
  ],
  status: Status14Enum.DELETED,
  trackingCategoryID: '000024cc-0000-0000-0000-000000000000',
};
```

