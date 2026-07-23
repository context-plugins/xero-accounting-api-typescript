
# Manual Journal

Find out more here: [http://developer.xero.com/documentation/api/manual-journals/](http://developer.xero.com/documentation/api/manual-journals/)

## Structure

`ManualJournal`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `attachments` | [`Attachment[] \| undefined`](../../doc/models/attachment.md) | Optional | Displays array of attachments from the API |
| `date` | `string \| undefined` | Optional | Date journal was posted – YYYY-MM-DD |
| `hasAttachments` | `boolean \| undefined` | Optional, Read-only | Boolean to indicate if a manual journal has an attachment<br><br>**Default**: `false` |
| `journalLines` | [`ManualJournalLine[] \| undefined`](../../doc/models/manual-journal-line.md) | Optional | See JournalLines |
| `lineAmountTypes` | [`LineAmountTypesEnum \| undefined`](../../doc/models/line-amount-types-enum.md) | Optional | Line amounts are exclusive of tax by default if you don’t specify this element. See Line Amount Types |
| `manualJournalID` | `string \| undefined` | Optional | The Xero identifier for a Manual Journal |
| `narration` | `string` | Required | Description of journal being posted |
| `showOnCashBasisReports` | `boolean \| undefined` | Optional | Boolean – default is true if not specified |
| `status` | [`Status16Enum \| undefined`](../../doc/models/status-16-enum.md) | Optional | See Manual Journal Status Codes |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `url` | `string \| undefined` | Optional | Url link to a source document – shown as “Go to [appName]” in the Xero app |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |
| `warnings` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of warning messages from the API |

## Example

```ts
import { LineAmountTypesEnum, ManualJournal } from 'xero-accounting-apilib';

const manualJournal: ManualJournal = {
  narration: 'Narration2',
  attachments: [
    {
      attachmentID: '00000714-0000-0000-0000-000000000000',
      contentLength: 34,
      fileName: 'FileName6',
      includeOnline: false,
      mimeType: 'MimeType6',
    },
    {
      attachmentID: '00000714-0000-0000-0000-000000000000',
      contentLength: 34,
      fileName: 'FileName6',
      includeOnline: false,
      mimeType: 'MimeType6',
    }
  ],
  date: 'Date2',
  hasAttachments: false,
  journalLines: [
    {
      accountCode: 'AccountCode2',
      accountID: '000025e8-0000-0000-0000-000000000000',
      description: 'Description2',
      isBlank: false,
      lineAmount: 127.64,
    },
    {
      accountCode: 'AccountCode2',
      accountID: '000025e8-0000-0000-0000-000000000000',
      description: 'Description2',
      isBlank: false,
      lineAmount: 127.64,
    }
  ],
  lineAmountTypes: LineAmountTypesEnum.Exclusive,
  statusAttributeString: 'ERROR',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

