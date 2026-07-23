
# Conversion Date

The date when the organisation starts using Xero

## Structure

`ConversionDate`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `month` | `number \| undefined` | Optional | The month the organisation starts using Xero. Value is an integer between 1 and 12 |
| `year` | `number \| undefined` | Optional | The year the organisation starts using Xero. Value is an integer greater than 2006 |

## Example

```ts
import { ConversionDate } from 'xero-accounting-apilib';

const conversionDate: ConversionDate = {
  month: 1,
  year: 2020,
};
```

