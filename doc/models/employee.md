
# Employee

Find out more here: [http://developer.xero.com/documentation/api/employees/](http://developer.xero.com/documentation/api/employees/)

## Structure

`Employee`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `employeeID` | `string \| undefined` | Optional | The Xero identifier for an employee e.g. 297c2dc5-cc47-4afd-8ec8-74990b8761e9 |
| `externalLink` | [`ExternalLink \| undefined`](../../doc/models/external-link.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/) |
| `firstName` | `string \| undefined` | Optional | First name of an employee (max length = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `lastName` | `string \| undefined` | Optional | Last name of an employee (max length = 255)<br><br>**Constraints**: *Maximum Length*: `255` |
| `status` | [`Status10Enum \| undefined`](../../doc/models/status-10-enum.md) | Optional | Current status of an employee – see contact status types |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | - |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import { Employee, LinkTypeEnum, Status10Enum } from 'xero-accounting-apilib';

const employee: Employee = {
  employeeID: '000025ae-0000-0000-0000-000000000000',
  externalLink: {
    description: 'Description8',
    linkType: LinkTypeEnum.Twitter,
    url: 'Url4',
  },
  firstName: 'FirstName6',
  lastName: 'LastName6',
  status: Status10Enum.ACTIVE,
  statusAttributeString: 'ERROR',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

