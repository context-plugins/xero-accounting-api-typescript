
# Tracking Categories

## Structure

`TrackingCategories`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `trackingCategories` | [`TrackingCategory[] \| undefined`](../../doc/models/tracking-category.md) | Optional | - |

## Example

```ts
import {
  Status13Enum,
  Status14Enum,
  TrackingCategories,
} from 'xero-accounting-apilib';

const trackingCategories: TrackingCategories = {
  trackingCategories: [
    {
      name: 'Name6',
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
      status: Status14Enum.ACTIVE,
      trackingCategoryID: '0000262a-0000-0000-0000-000000000000',
    },
    {
      name: 'Name6',
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
      status: Status14Enum.ACTIVE,
      trackingCategoryID: '0000262a-0000-0000-0000-000000000000',
    },
    {
      name: 'Name6',
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
      status: Status14Enum.ACTIVE,
      trackingCategoryID: '0000262a-0000-0000-0000-000000000000',
    }
  ],
};
```

