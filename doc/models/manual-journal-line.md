
# Manual Journal Line

Find out more here: [http://developer.xero.com/documentation/api/manual-journals/](http://developer.xero.com/documentation/api/manual-journals/)

## Structure

`ManualJournalLine`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountCode` | `string \| undefined` | Optional | See Accounts |
| `accountID` | `string \| undefined` | Optional | See Accounts |
| `description` | `string \| undefined` | Optional | Description for journal line |
| `isBlank` | `boolean \| undefined` | Optional | is the line blank |
| `lineAmount` | `number \| undefined` | Optional | total for line. Debits are positive, credits are negative value |
| `taxAmount` | `number \| undefined` | Optional, Read-only | The calculated tax amount based on the TaxType and LineAmount |
| `taxType` | `string \| undefined` | Optional | The tax type from TaxRates |
| `tracking` | [`TrackingCategory[] \| undefined`](../../doc/models/tracking-category.md) | Optional | Optional Tracking Category – see Tracking. Any JournalLine can have a maximum of 2 <TrackingCategory> elements. |

## Example

```ts
import { ManualJournalLine } from 'xero-accounting-apilib';

const manualJournalLine: ManualJournalLine = {
  accountCode: '720',
  accountID: '000019e2-0000-0000-0000-000000000000',
  description: 'Coded incorrectly Office Equipment should be Computer Equipment',
  isBlank: false,
  lineAmount: -2569,
  taxAmount: 0,
};
```

