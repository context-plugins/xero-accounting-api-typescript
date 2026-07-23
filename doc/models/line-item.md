
# Line Item

Find out more here: [https://developer.xero.com/documentation/api/invoices#post](https://developer.xero.com/documentation/api/invoices#post)

## Structure

`LineItem`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountCode` | `string \| undefined` | Optional | See Accounts |
| `description` | `string \| undefined` | Optional | Description needs to be at least 1 char long. A line item with just a description (i.e no unit amount or quantity) can be created by specifying just a <Description> element that contains at least 1 character |
| `discountAmount` | `number \| undefined` | Optional | Discount amount being applied to a line item. Only supported on ACCREC invoices - ACCPAY invoices and credit notes in Xero do not support discounts. |
| `discountRate` | `number \| undefined` | Optional | Percentage discount being applied to a line item (only supported on  ACCREC invoices – ACC PAY invoices and credit notes in Xero do not support discounts |
| `itemCode` | `string \| undefined` | Optional | See Items |
| `lineAmount` | `number \| undefined` | Optional | If you wish to omit either of the <Quantity> or <UnitAmount> you can provide a LineAmount and Xero will calculate the missing amount for you. The line amount reflects the discounted price if a DiscountRate has been used . i.e LineAmount = Quantity * Unit Amount * ((100 – DiscountRate)/100) |
| `lineItemID` | `string \| undefined` | Optional | LineItem unique ID |
| `quantity` | `number \| undefined` | Optional | LineItem Quantity |
| `repeatingInvoiceID` | `string \| undefined` | Optional | The Xero identifier for a Repeating Invoice |
| `taxAmount` | `number \| undefined` | Optional | The tax amount is auto calculated as a percentage of the line amount (see below) based on the tax rate. This value can be overriden if the calculated <TaxAmount> is not correct. |
| `taxType` | `string \| undefined` | Optional | The tax type from TaxRates |
| `tracking` | [`LineItemTracking[] \| undefined`](../../doc/models/line-item-tracking.md) | Optional | Optional Tracking Category – see Tracking.  Any LineItem can have a  maximum of 2 <TrackingCategory> elements. |
| `unitAmount` | `number \| undefined` | Optional | LineItem Unit Amount |

## Example

```ts
import { LineItem } from 'xero-accounting-apilib';

const lineItem: LineItem = {
  accountCode: 'AccountCode0',
  description: 'Description0',
  discountAmount: 57.42,
  discountRate: 157.2,
  itemCode: 'ItemCode6',
  lineItemID: '00000000-0000-0000-0000-000000000000',
  repeatingInvoiceID: '00000000-0000-0000-0000-000000000000',
};
```

