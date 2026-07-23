
# Organisation Role Enum

User role that defines permissions in Xero and via API (READONLY, INVOICEONLY, STANDARD, FINANCIALADVISER, etc)

## Enumeration

`OrganisationRoleEnum`

## Fields

| Name |
|  --- |
| `READONLY` |
| `INVOICEONLY` |
| `STANDARD` |
| `FINANCIALADVISER` |
| `MANAGEDCLIENT` |
| `CASHBOOKCLIENT` |
| `UNKNOWN` |

## Example

```ts
import { OrganisationRoleEnum } from 'xero-accounting-apilib';

const organisationRole = OrganisationRoleEnum.INVOICEONLY;
```

