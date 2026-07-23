
# Contact

Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)

## Structure

`Contact`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountNumber` | `string \| undefined` | Optional | A user defined account number. This can be updated via the API and the Xero UI (max length = 50)<br><br>**Constraints**: *Maximum Length*: `50` |
| `accountsPayableTaxType` | `string \| undefined` | Optional | The tax type from TaxRates |
| `accountsReceivableTaxType` | `string \| undefined` | Optional | The tax type from TaxRates |
| `addresses` | [`Address[] \| undefined`](../../doc/models/address.md) | Optional | Store certain address types for a contact – see address types |
| `attachments` | [`Attachment[] \| undefined`](../../doc/models/attachment.md) | Optional | Displays array of attachments from the API |
| `balances` | [`Balances \| undefined`](../../doc/models/balances.md) | Optional | The raw AccountsReceivable(sales invoices) and AccountsPayable(bills) outstanding and overdue amounts, not converted to base currency (read only) |
| `bankAccountDetails` | `string \| undefined` | Optional | Bank account number of contact |
| `batchPayments` | [`BatchPaymentDetails \| undefined`](../../doc/models/batch-payment-details.md) | Optional | Bank details for use on a batch payment stored with each contact<br><br>Find out more here: [http://developer.xero.com/documentation/api/Contact/](http://developer.xero.com/documentation/api/Contact/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/Contact/](http://developer.xero.com/documentation/api/Contact/) |
| `brandingTheme` | [`BrandingTheme \| undefined`](../../doc/models/branding-theme.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/branding-themes/](http://developer.xero.com/documentation/api/branding-themes/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/branding-themes/](http://developer.xero.com/documentation/api/branding-themes/) |
| `contactGroups` | [`ContactGroup[] \| undefined`](../../doc/models/contact-group.md) | Optional | Displays which contact groups a contact is included in |
| `contactID` | `string \| undefined` | Optional | Xero identifier |
| `contactNumber` | `string \| undefined` | Optional | This can be updated via the API only i.e. This field is read only on the Xero contact screen, used to identify contacts in external systems (max length = 50). If the Contact Number is used, this is displayed as Contact Code in the Contacts UI in Xero.<br><br>**Constraints**: *Maximum Length*: `50` |
| `contactPersons` | [`ContactPerson[] \| undefined`](../../doc/models/contact-person.md) | Optional | See contact persons |
| `contactStatus` | [`ContactStatusEnum \| undefined`](../../doc/models/contact-status-enum.md) | Optional | Current status of a contact – see contact status types |
| `defaultCurrency` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `discount` | `number \| undefined` | Optional, Read-only | The default discount rate for the contact (read only) |
| `emailAddress` | `string \| undefined` | Optional | Email address of contact person (umlauts not supported) (max length  = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `firstName` | `string \| undefined` | Optional | First name of contact person (max length = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `hasAttachments` | `boolean \| undefined` | Optional | A boolean to indicate if a contact has an attachment<br><br>**Default**: `false` |
| `hasValidationErrors` | `boolean \| undefined` | Optional | A boolean to indicate if a contact has an validation errors<br><br>**Default**: `false` |
| `isCustomer` | `boolean \| undefined` | Optional | true or false – Boolean that describes if a contact has any AR invoices entered against them. Cannot be set via PUT or POST – it is automatically set when an accounts receivable invoice is generated against this contact. |
| `isSupplier` | `boolean \| undefined` | Optional | true or false – Boolean that describes if a contact that has any AP  invoices entered against them. Cannot be set via PUT or POST – it is automatically set when an accounts payable invoice is generated against this contact. |
| `lastName` | `string \| undefined` | Optional | Last name of contact person (max length = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `name` | `string \| undefined` | Optional | Full name of contact/organisation (max length = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `paymentTerms` | [`PaymentTerm \| undefined`](../../doc/models/payment-term.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/) |
| `phones` | [`Phone[] \| undefined`](../../doc/models/phone.md) | Optional | Store certain phone types for a contact – see phone types |
| `purchasesDefaultAccountCode` | `string \| undefined` | Optional | The default purchases account code for contacts |
| `purchasesTrackingCategories` | [`SalesTrackingCategory[] \| undefined`](../../doc/models/sales-tracking-category.md) | Optional | The default purchases tracking categories for contacts |
| `salesDefaultAccountCode` | `string \| undefined` | Optional | The default sales account code for contacts |
| `salesTrackingCategories` | [`SalesTrackingCategory[] \| undefined`](../../doc/models/sales-tracking-category.md) | Optional | The default sales tracking categories for contacts |
| `skypeUserName` | `string \| undefined` | Optional | Skype user name of contact |
| `statusAttributeString` | `string \| undefined` | Optional | Status of object |
| `taxNumber` | `string \| undefined` | Optional | Tax number of contact – this is also known as the ABN (Australia), GST Number (New Zealand), VAT Number (UK) or Tax ID Number (US and global) in the Xero UI depending on which regionalized version of Xero you are using (max length = 50)<br><br>**Constraints**: *Maximum Length*: `50` |
| `trackingCategoryName` | `string \| undefined` | Optional | The name of the Tracking Category assigned to the contact under SalesTrackingCategories and PurchasesTrackingCategories |
| `trackingCategoryOption` | `string \| undefined` | Optional | The name of the Tracking Option assigned to the contact under SalesTrackingCategories and PurchasesTrackingCategories |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of last update to contact |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays validation errors returned from the API |
| `website` | `string \| undefined` | Optional, Read-only | Website address for contact (read only) |
| `xeroNetworkKey` | `string \| undefined` | Optional | Store XeroNetworkKey for contacts. |

## Example

```ts
import { AddressTypeEnum, Contact } from 'xero-accounting-apilib';

const contact: Contact = {
  accountNumber: 'AccountNumber6',
  accountsPayableTaxType: 'AccountsPayableTaxType6',
  accountsReceivableTaxType: 'AccountsReceivableTaxType2',
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
  hasAttachments: false,
  hasValidationErrors: false,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

