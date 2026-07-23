
# User

Find out more here: [http://developer.xero.com/documentation/api/users/](http://developer.xero.com/documentation/api/users/)

## Structure

`User`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `emailAddress` | `string \| undefined` | Optional | Email address of user |
| `firstName` | `string \| undefined` | Optional | First name of user |
| `isSubscriber` | `boolean \| undefined` | Optional | Boolean to indicate if user is the subscriber |
| `lastName` | `string \| undefined` | Optional | Last name of user |
| `organisationRole` | [`OrganisationRoleEnum \| undefined`](../../doc/models/organisation-role-enum.md) | Optional | User role that defines permissions in Xero and via API (READONLY, INVOICEONLY, STANDARD, FINANCIALADVISER, etc) |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Timestamp of last change to user |
| `userID` | `string \| undefined` | Optional | Xero identifier |

## Example

```ts
import { OrganisationRoleEnum, User } from 'xero-accounting-apilib';

const user: User = {
  emailAddress: 'EmailAddress6',
  firstName: 'FirstName4',
  isSubscriber: false,
  lastName: 'LastName4',
  organisationRole: OrganisationRoleEnum.STANDARD,
  updatedDateUTC: '/Date(1573755038314)/',
};
```

