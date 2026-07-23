
# Item

Find out more here: [http://developer.xero.com/documentation/api/items/](http://developer.xero.com/documentation/api/items/)

## Structure

`Item`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `code` | `string` | Required | User defined item code (max length = 30)<br><br>**Constraints**: *Maximum Length*: `30` |
| `description` | `string \| undefined` | Optional | The sales description of the item (max length = 4000)<br><br>**Constraints**: *Maximum Length*: `4000` |
| `inventoryAssetAccountCode` | `string \| undefined` | Optional | The inventory asset account for the item. The account must be of type INVENTORY. The  COGSAccountCode in PurchaseDetails is also required to create a tracked item |
| `isPurchased` | `boolean \| undefined` | Optional | Boolean value, defaults to true. When IsPurchased is true the item is available for purchase transactions in the Xero UI. If IsPurchased is updated to false then PurchaseDescription and PurchaseDetails values will be nulled. |
| `isSold` | `boolean \| undefined` | Optional | Boolean value, defaults to true. When IsSold is true the item will be available on sales transactions in the Xero UI. If IsSold is updated to false then Description and SalesDetails values will be nulled. |
| `isTrackedAsInventory` | `boolean \| undefined` | Optional | True for items that are tracked as inventory. An item will be tracked as inventory if the InventoryAssetAccountCode and COGSAccountCode are set. |
| `itemID` | `string \| undefined` | Optional | The Xero identifier for an Item |
| `name` | `string \| undefined` | Optional | The name of the item (max length = 50)<br><br>**Constraints**: *Maximum Length*: `50` |
| `purchaseDescription` | `string \| undefined` | Optional | The purchase description of the item (max length = 4000)<br><br>**Constraints**: *Maximum Length*: `4000` |
| `purchaseDetails` | [`Purchase \| undefined`](../../doc/models/purchase.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/items/](http://developer.xero.com/documentation/api/items/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/items/](http://developer.xero.com/documentation/api/items/) |
| `quantityOnHand` | `number \| undefined` | Optional | The quantity of the item on hand |
| `salesDetails` | [`Purchase \| undefined`](../../doc/models/purchase.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/items/](http://developer.xero.com/documentation/api/items/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/items/](http://developer.xero.com/documentation/api/items/) |
| `statusAttributeString` | `string \| undefined` | Optional | Status of object |
| `totalCostPool` | `number \| undefined` | Optional | The value of the item on hand. Calculated using average cost accounting. |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date in UTC format |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import { Item } from 'xero-accounting-apilib';

const item: Item = {
  code: 'Code2',
  description: 'Description6',
  inventoryAssetAccountCode: 'InventoryAssetAccountCode8',
  isPurchased: false,
  isSold: false,
  isTrackedAsInventory: false,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

