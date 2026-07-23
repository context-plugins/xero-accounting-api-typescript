
# Purchase Order

Find out more here: [http://developer.xero.com/documentation/api/purchase-orders/](http://developer.xero.com/documentation/api/purchase-orders/)

## Structure

`PurchaseOrder`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `attachments` | [`Attachment[] \| undefined`](../../doc/models/attachment.md) | Optional | Displays array of attachments from the API |
| `attentionTo` | `string \| undefined` | Optional | The person that the delivery is going to |
| `brandingThemeID` | `string \| undefined` | Optional | See BrandingThemes |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `currencyCode` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `currencyRate` | `number \| undefined` | Optional | The currency rate for a multicurrency purchase order. If no rate is specified, the XE.com day rate is used. |
| `date` | `string \| undefined` | Optional | Date purchase order was issued – YYYY-MM-DD. If the Date element is not specified then it will default to the current date based on the timezone setting of the organisation |
| `deliveryAddress` | `string \| undefined` | Optional | The address the goods are to be delivered to |
| `deliveryDate` | `string \| undefined` | Optional | Date the goods are to be delivered – YYYY-MM-DD |
| `deliveryInstructions` | `string \| undefined` | Optional | A free text feild for instructions (500 characters max) |
| `expectedArrivalDate` | `string \| undefined` | Optional | The date the goods are expected to arrive. |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if a purchase order has an attachment<br><br>**Default**: `false` |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[] \| undefined`](../../doc/models/line-item.md) | Optional | See LineItems |
| `purchaseOrderID` | `string \| undefined` | Optional | Xero generated unique identifier for purchase order |
| `purchaseOrderNumber` | `string \| undefined` | Optional | Unique alpha numeric code identifying purchase order (when missing will auto-generate from your Organisation Invoice Settings) |
| `reference` | `string \| undefined` | Optional | Additional reference number |
| `sentToContact` | `boolean \| undefined` | Optional | Boolean to set whether the purchase order should be marked as “sent”. This can be set only on purchase orders that have been approved or billed |
| `status` | [`Status17Enum \| undefined`](../../doc/models/status-17-enum.md) | Optional | See Purchase Order Status Codes |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `subTotal` | `number \| undefined` | Optional, Read-only | Total of purchase order excluding taxes |
| `telephone` | `string \| undefined` | Optional | The phone number for the person accepting the delivery |
| `total` | `number \| undefined` | Optional, Read-only | Total of Purchase Order tax inclusive (i.e. SubTotal + TotalTax) |
| `totalDiscount` | `number \| undefined` | Optional, Read-only | Total of discounts applied on the purchase order line items |
| `totalTax` | `number \| undefined` | Optional, Read-only | Total tax on purchase order |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |
| `warnings` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of warning messages from the API |

## Example

```ts
import {
  AddressTypeEnum,
  CurrencyCodeEnum,
  PurchaseOrder,
} from 'xero-accounting-apilib';

const purchaseOrder: PurchaseOrder = {
  attachments: [
    {
      attachmentID: '00000714-0000-0000-0000-000000000000',
      contentLength: 34,
      fileName: 'FileName6',
      includeOnline: false,
      mimeType: 'MimeType6',
    }
  ],
  attentionTo: 'AttentionTo0',
  brandingThemeID: '0000007a-0000-0000-0000-000000000000',
  contact: {
    accountNumber: 'AccountNumber2',
    accountsPayableTaxType: 'AccountsPayableTaxType2',
    accountsReceivableTaxType: 'AccountsReceivableTaxType6',
    addresses: [
      {
        addressLine1: 'AddressLine14',
        addressLine2: 'AddressLine20',
        addressLine3: 'AddressLine38',
        addressLine4: 'AddressLine46',
        addressType: AddressTypeEnum.POBOX,
      }
    ],
    attachments: [
      {
        attachmentID: '00000714-0000-0000-0000-000000000000',
        contentLength: 34,
        fileName: 'FileName6',
        includeOnline: false,
        mimeType: 'MimeType6',
      },
      {
        attachmentID: '00000714-0000-0000-0000-000000000000',
        contentLength: 34,
        fileName: 'FileName6',
        includeOnline: false,
        mimeType: 'MimeType6',
      }
    ],
  },
  currencyCode: CurrencyCodeEnum.NIO,
  hasAttachments: false,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

