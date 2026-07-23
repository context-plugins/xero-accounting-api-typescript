
# Employees

## Structure

`Employees`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `employees` | [`Employee[] \| undefined`](../../doc/models/employee.md) | Optional | - |

## Example

```ts
import {
  Employees,
  LinkTypeEnum,
  Status10Enum,
} from 'xero-accounting-apilib';

const employees: Employees = {
  employees: [
    {
      employeeID: '000009cc-0000-0000-0000-000000000000',
      externalLink: {
        description: 'Description8',
        linkType: LinkTypeEnum.Twitter,
        url: 'Url4',
      },
      firstName: 'FirstName8',
      lastName: 'LastName8',
      status: Status10Enum.GDPRREQUEST,
    }
  ],
};
```

