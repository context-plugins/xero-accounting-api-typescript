
# Line Item Tracking

Find out more here: [https://developer.xero.com/documentation/api/invoices#post](https://developer.xero.com/documentation/api/invoices#post)

## Structure

`LineItemTracking`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string \| undefined` | Optional | The name of the tracking category<br><br>**Constraints**: *Maximum Length*: `100` |
| `option` | `string \| undefined` | Optional | See Tracking Options |
| `trackingCategoryID` | `string \| undefined` | Optional | The Xero identifier for a tracking category |
| `trackingOptionID` | `string \| undefined` | Optional | The Xero identifier for a tracking category option |

## Example

```ts
import { LineItemTracking } from 'xero-accounting-apilib';

const lineItemTracking: LineItemTracking = {
  name: 'Region',
  option: 'North',
  trackingCategoryID: '00000000-0000-0000-0000-000000000000',
  trackingOptionID: '00000000-0000-0000-0000-000000000000',
};
```

