
# Journal

Find out more here: [http://developer.xero.com/documentation/api/journals/](http://developer.xero.com/documentation/api/journals/)

## Structure

`Journal`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `createdDateUTC` | `string \| undefined` | Optional, Read-only | Created date UTC format |
| `journalDate` | `string \| undefined` | Optional | Date the journal was posted |
| `journalID` | `string \| undefined` | Optional | Xero identifier |
| `journalLines` | [`JournalLine[] \| undefined`](../../doc/models/journal-line.md) | Optional | See JournalLines |
| `journalNumber` | `number \| undefined` | Optional | Xero generated journal number |
| `reference` | `string \| undefined` | Optional | reference field for additional indetifying information |
| `sourceID` | `string \| undefined` | Optional | The identifier for the source transaction (e.g. InvoiceID) |
| `sourceType` | [`SourceTypeEnum \| undefined`](../../doc/models/source-type-enum.md) | Optional | The journal source type. The type of transaction that created the journal |

## Example

```ts
import { AccountTypeEnum, Journal } from 'xero-accounting-apilib';

const journal: Journal = {
  createdDateUTC: '/Date(1573755038314)/',
  journalDate: 'JournalDate6',
  journalID: '000021ec-0000-0000-0000-000000000000',
  journalLines: [
    {
      accountCode: 'AccountCode2',
      accountID: '000025e8-0000-0000-0000-000000000000',
      accountName: 'AccountName8',
      accountType: AccountTypeEnum.EXPENSE,
      description: 'Description2',
    },
    {
      accountCode: 'AccountCode2',
      accountID: '000025e8-0000-0000-0000-000000000000',
      accountName: 'AccountName8',
      accountType: AccountTypeEnum.EXPENSE,
      description: 'Description2',
    },
    {
      accountCode: 'AccountCode2',
      accountID: '000025e8-0000-0000-0000-000000000000',
      accountName: 'AccountName8',
      accountType: AccountTypeEnum.EXPENSE,
      description: 'Description2',
    }
  ],
  journalNumber: 90,
};
```

