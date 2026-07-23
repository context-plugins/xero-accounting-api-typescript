
# Journals

## Structure

`Journals`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `journals` | [`Journal[] \| undefined`](../../doc/models/journal.md) | Optional | - |

## Example

```ts
import { AccountTypeEnum, Journals } from 'xero-accounting-apilib';

const journals: Journals = {
  journals: [
    {
      createdDateUTC: 'CreatedDateUTC6',
      journalDate: 'JournalDate6',
      journalID: '00002578-0000-0000-0000-000000000000',
      journalLines: [
        {
          accountCode: 'AccountCode2',
          accountID: '000025e8-0000-0000-0000-000000000000',
          accountName: 'AccountName8',
          accountType: AccountTypeEnum.EXPENSE,
          description: 'Description2',
        }
      ],
      journalNumber: 166,
    },
    {
      createdDateUTC: 'CreatedDateUTC6',
      journalDate: 'JournalDate6',
      journalID: '00002578-0000-0000-0000-000000000000',
      journalLines: [
        {
          accountCode: 'AccountCode2',
          accountID: '000025e8-0000-0000-0000-000000000000',
          accountName: 'AccountName8',
          accountType: AccountTypeEnum.EXPENSE,
          description: 'Description2',
        }
      ],
      journalNumber: 166,
    },
    {
      createdDateUTC: 'CreatedDateUTC6',
      journalDate: 'JournalDate6',
      journalID: '00002578-0000-0000-0000-000000000000',
      journalLines: [
        {
          accountCode: 'AccountCode2',
          accountID: '000025e8-0000-0000-0000-000000000000',
          accountName: 'AccountName8',
          accountType: AccountTypeEnum.EXPENSE,
          description: 'Description2',
        }
      ],
      journalNumber: 166,
    }
  ],
};
```

