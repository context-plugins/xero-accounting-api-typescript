
# Contact Group

Find out more here: [http://developer.xero.com/documentation/api/contactgroups/](http://developer.xero.com/documentation/api/contactgroups/)

## Structure

`ContactGroup`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `contactGroupID` | `string \| undefined` | Optional | The Xero identifier for an contact group – specified as a string following the endpoint name. e.g. /297c2dc5-cc47-4afd-8ec8-74990b8761e9 |
| `contacts` | [`Contact[] \| undefined`](../../doc/models/contact.md) | Optional | The ContactID and Name of Contacts in a contact group. Returned on GETs when the ContactGroupID is supplied in the URL. |
| `name` | `string \| undefined` | Optional | The Name of the contact group. Required when creating a new contact  group |
| `status` | [`Status2Enum \| undefined`](../../doc/models/status-2-enum.md) | Optional | The Status of a contact group. To delete a contact group update the status to DELETED. Only contact groups with a status of ACTIVE are returned on GETs. |

## Example

```ts
import {
  AddressTypeEnum,
  ContactGroup,
  Status2Enum,
} from 'xero-accounting-apilib';

const contactGroup: ContactGroup = {
  contactGroupID: '000001e2-0000-0000-0000-000000000000',
  contacts: [
    {
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
    },
    {
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
    },
    {
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
    }
  ],
  name: 'Name8',
  status: Status2Enum.ACTIVE,
};
```

