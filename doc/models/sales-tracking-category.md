
# Sales Tracking Category

Find out more here: [http://developer.xero.com/documentation/api/tracking-categories/](http://developer.xero.com/documentation/api/tracking-categories/)

## Structure

`SalesTrackingCategory`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `trackingCategoryName` | `string \| undefined` | Optional | The default sales tracking category name for contacts |
| `trackingOptionName` | `string \| undefined` | Optional | The default purchase tracking category name for contacts |

## Example

```ts
import { SalesTrackingCategory } from 'xero-accounting-apilib';

const salesTrackingCategory: SalesTrackingCategory = {
  trackingCategoryName: 'TrackingCategoryName0',
  trackingOptionName: 'TrackingOptionName8',
};
```

