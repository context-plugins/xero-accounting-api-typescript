
# Items

## Structure

`Items`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `items` | [`Item[] \| undefined`](../../doc/models/item.md) | Optional | - |

## Example

```ts
import { Items } from 'xero-accounting-apilib';

const items: Items = {
  items: [
    {
      code: 'Code0',
      description: 'Description6',
      inventoryAssetAccountCode: 'InventoryAssetAccountCode4',
      isPurchased: false,
      isSold: false,
      isTrackedAsInventory: false,
    },
    {
      code: 'Code0',
      description: 'Description6',
      inventoryAssetAccountCode: 'InventoryAssetAccountCode4',
      isPurchased: false,
      isSold: false,
      isTrackedAsInventory: false,
    }
  ],
};
```

