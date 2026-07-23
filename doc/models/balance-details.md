
# Balance Details

An array to specify multiple currency balances of an account

## Structure

`BalanceDetails`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `balance` | `number \| undefined` | Optional | The opening balances of the account. Debits are positive, credits are negative values |
| `currencyCode` | `string \| undefined` | Optional | The currency of the balance (Not required for base currency) |
| `currencyRate` | `number \| undefined` | Optional | (Optional) Exchange rate to base currency when money is spent or received. If not specified, XE rate for the day is applied |

## Example

```ts
import { BalanceDetails } from 'xero-accounting-apilib';

const balanceDetails: BalanceDetails = {
  balance: 101.08,
  currencyCode: 'CurrencyCode0',
  currencyRate: 146.4,
};
```

