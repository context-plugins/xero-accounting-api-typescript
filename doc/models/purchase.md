
# Purchase

Find out more here: [http://developer.xero.com/documentation/api/items/](http://developer.xero.com/documentation/api/items/)

## Structure

`Purchase`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountCode` | `string \| undefined` | Optional | Default account code to be used for purchased/sale. Not applicable to the purchase details of tracked items |
| `cOGSAccountCode` | `string \| undefined` | Optional | Cost of goods sold account. Only applicable to the purchase details of tracked items. |
| `taxType` | `string \| undefined` | Optional | The tax type from TaxRates |
| `unitPrice` | `number \| undefined` | Optional | Unit Price of the item. By default UnitPrice is rounded to two decimal places. You can use 4 decimal places by adding the unitdp=4 querystring parameter to your request. |

## Example

```ts
import { Purchase } from 'xero-accounting-apilib';

const purchase: Purchase = {
  accountCode: 'AccountCode8',
  cOGSAccountCode: 'COGSAccountCode0',
  taxType: 'TaxType2',
  unitPrice: 70.48,
};
```

