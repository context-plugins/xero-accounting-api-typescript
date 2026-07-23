
# Contact Person

Find out more here: [http://developer.xero.com/documentation/api/contacts/](http://developer.xero.com/documentation/api/contacts/)

## Structure

`ContactPerson`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `emailAddress` | `string \| undefined` | Optional | Email address of person |
| `firstName` | `string \| undefined` | Optional | First name of person |
| `includeInEmails` | `boolean \| undefined` | Optional | boolean to indicate whether contact should be included on emails with invoices etc. |
| `lastName` | `string \| undefined` | Optional | Last name of person |

## Example

```ts
import { ContactPerson } from 'xero-accounting-apilib';

const contactPerson: ContactPerson = {
  emailAddress: 'EmailAddress6',
  firstName: 'FirstName4',
  includeInEmails: false,
  lastName: 'LastName4',
};
```

