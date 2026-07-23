
# Users

## Structure

`Users`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `users` | [`User[] \| undefined`](../../doc/models/user.md) | Optional | - |

## Example

```ts
import { OrganisationRoleEnum, Users } from 'xero-accounting-apilib';

const users: Users = {
  users: [
    {
      emailAddress: 'EmailAddress0',
      firstName: 'FirstName0',
      isSubscriber: false,
      lastName: 'LastName0',
      organisationRole: OrganisationRoleEnum.READONLY,
    }
  ],
};
```

