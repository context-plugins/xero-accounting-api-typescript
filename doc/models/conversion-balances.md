
# Conversion Balances

Balance supplied for each account that has a value as at the conversion date.

## Structure

`ConversionBalances`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accountCode` | `string \| undefined` | Optional | The account code for a account |
| `balance` | `number \| undefined` | Optional | The opening balances of the account. Debits are positive, credits are negative values |
| `balanceDetails` | [`BalanceDetails[] \| undefined`](../../doc/models/balance-details.md) | Optional | - |

## Example

```ts
import { ConversionBalances } from 'xero-accounting-apilib';

const conversionBalances: ConversionBalances = {
  accountCode: 'AccountCode0',
  balance: 134.94,
  balanceDetails: [
    {
      balance: 162.9,
      currencyCode: 'CurrencyCode2',
      currencyRate: 208.22,
    },
    {
      balance: 162.9,
      currencyCode: 'CurrencyCode2',
      currencyRate: 208.22,
    }
  ],
};
```

