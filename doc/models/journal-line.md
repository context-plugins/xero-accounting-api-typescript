
# Journal Line

Find out more here: [https://developer.xero.com/documentation/api/journals#JournalLines](https://developer.xero.com/documentation/api/journals#JournalLines)

## Structure

`JournalLine`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountCode` | `string \| undefined` | Optional | See Accounts |
| `accountID` | `string \| undefined` | Optional | See Accounts |
| `accountName` | `string \| undefined` | Optional | See AccountCodes |
| `accountType` | [`AccountTypeEnum \| undefined`](../../doc/models/account-type-enum.md) | Optional | See Account Types |
| `description` | `string \| undefined` | Optional | The description from the source transaction line item. Only returned if populated. |
| `grossAmount` | `number \| undefined` | Optional | Gross amount of journal line (NetAmount + TaxAmount). |
| `journalLineID` | `string \| undefined` | Optional | Xero identifier for Journal |
| `netAmount` | `number \| undefined` | Optional | Net amount of journal line. This will be a positive value for a debit and negative for a credit |
| `taxAmount` | `number \| undefined` | Optional, Read-only | Total tax on a journal line |
| `taxName` | `string \| undefined` | Optional | see TaxRates |
| `taxType` | `string \| undefined` | Optional | The tax type from TaxRates |
| `trackingCategories` | [`TrackingCategory[] \| undefined`](../../doc/models/tracking-category.md) | Optional | Optional Tracking Category – see Tracking. Any JournalLine can have a maximum of 2 <TrackingCategory> elements. |

## Example

```ts
import { AccountTypeEnum, JournalLine } from 'xero-accounting-apilib';

const journalLine: JournalLine = {
  accountCode: '90',
  accountID: 'ceef66a5-a545-413b-9312-78a53caadbc4',
  accountName: 'Checking Account',
  accountType: AccountTypeEnum.DIRECTCOSTS,
  description: 'My business checking account',
  grossAmount: 4130.98,
  journalLineID: '7be9db36-3598-4755-ba5c-c2dbc8c4a7a2',
  netAmount: 4130.98,
  taxAmount: 0,
  taxName: 'Tax Exempt',
};
```

