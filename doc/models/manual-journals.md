
# Manual Journals

## Structure

`ManualJournals`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `manualJournals` | [`ManualJournal[] \| undefined`](../../doc/models/manual-journal.md) | Optional | - |

## Example

```ts
import { LineAmountTypesEnum, ManualJournals } from 'xero-accounting-apilib';

const manualJournals: ManualJournals = {
  manualJournals: [
    {
      narration: 'Narration6',
      attachments: [
        {
          attachmentID: '00000714-0000-0000-0000-000000000000',
          contentLength: 34,
          fileName: 'FileName6',
          includeOnline: false,
          mimeType: 'MimeType6',
        }
      ],
      date: 'Date6',
      hasAttachments: false,
      journalLines: [
        {
          accountCode: 'AccountCode2',
          accountID: '000025e8-0000-0000-0000-000000000000',
          description: 'Description2',
          isBlank: false,
          lineAmount: 127.64,
        }
      ],
      lineAmountTypes: LineAmountTypesEnum.NoTax,
    },
    {
      narration: 'Narration6',
      attachments: [
        {
          attachmentID: '00000714-0000-0000-0000-000000000000',
          contentLength: 34,
          fileName: 'FileName6',
          includeOnline: false,
          mimeType: 'MimeType6',
        }
      ],
      date: 'Date6',
      hasAttachments: false,
      journalLines: [
        {
          accountCode: 'AccountCode2',
          accountID: '000025e8-0000-0000-0000-000000000000',
          description: 'Description2',
          isBlank: false,
          lineAmount: 127.64,
        }
      ],
      lineAmountTypes: LineAmountTypesEnum.NoTax,
    }
  ],
};
```

