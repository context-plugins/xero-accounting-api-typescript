
# Tracking Option

Find out more here: [http://developer.xero.com/documentation/api/tracking-categories/](http://developer.xero.com/documentation/api/tracking-categories/)

## Structure

`TrackingOption`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string \| undefined` | Optional | The name of the tracking option e.g. Marketing, East (max length = 100)<br><br>**Constraints**: *Maximum Length*: `100` |
| `status` | [`Status13Enum \| undefined`](../../doc/models/status-13-enum.md) | Optional | The status of a tracking option |
| `trackingCategoryID` | `string \| undefined` | Optional | Filter by a tracking category e.g. 297c2dc5-cc47-4afd-8ec8-74990b8761e9 |
| `trackingOptionID` | `string \| undefined` | Optional | The Xero identifier for a tracking option e.g. ae777a87-5ef3-4fa0-a4f0-d10e1f13073a |

## Example

```ts
import { Status13Enum, TrackingOption } from 'xero-accounting-apilib';

const trackingOption: TrackingOption = {
  name: 'Name6',
  status: Status13Enum.ARCHIVED,
  trackingCategoryID: '0000259e-0000-0000-0000-000000000000',
  trackingOptionID: '00001a06-0000-0000-0000-000000000000',
};
```

