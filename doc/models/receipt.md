
# Receipt

Find out more here: [http://developer.xero.com/documentation/api/receipts/](http://developer.xero.com/documentation/api/receipts/)

## Structure

`Receipt`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `attachments` | [`Attachment[] \| undefined`](../../doc/models/attachment.md) | Optional | Displays array of attachments from the API |
| `contact` | [`Contact \| undefined`](../../doc/models/contact.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/) |
| `date` | `string \| undefined` | Optional | Date of receipt – YYYY-MM-DD |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | boolean to indicate if a receipt has an attachment<br><br>**Default**: `false` |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `lineItems` | [`LineItem[] \| undefined`](../../doc/models/line-item.md) | Optional | - |
| `receiptID` | `string \| undefined` | Optional | Xero generated unique identifier for receipt |
| `receiptNumber` | `string \| undefined` | Optional, Read-only | Xero generated sequence number for receipt in current claim for a given user |
| `reference` | `string \| undefined` | Optional | Additional reference number |
| `status` | [`Status11Enum \| undefined`](../../doc/models/status-11-enum.md) | Optional | Current status of receipt – see status types |
| `subTotal` | `number \| undefined` | Optional | Total of receipt excluding taxes |
| `total` | `number \| undefined` | Optional | Total of receipt tax inclusive (i.e. SubTotal + TotalTax) |
| `totalTax` | `number \| undefined` | Optional | Total tax on receipt |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `url` | `string \| undefined` | Optional, Read-only | URL link to a source document – shown as “Go to [appName]” in the Xero app |
| `user` | [`User \| undefined`](../../doc/models/user.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/users/](http://developer.xero.com/documentation/api/users/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/users/](http://developer.xero.com/documentation/api/users/) |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |
| `warnings` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of warning messages from the API |

## Example

```ts
import {
  AddressTypeEnum,
  LineAmountTypesEnum,
  Receipt,
} from 'xero-accounting-apilib';

const receipt: Receipt = {
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
  date: 'Date2',
  hasAttachments: false,
  lineAmountTypes: LineAmountTypesEnum.Exclusive,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

