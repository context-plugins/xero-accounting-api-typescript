
# Setup

Find out more here: [https://developer.xero.com/documentation/api-guides/conversions](https://developer.xero.com/documentation/api-guides/conversions)

## Structure

`Setup`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accounts` | [`Account[] \| undefined`](../../doc/models/account.md) | Optional | - |
| `conversionBalances` | [`ConversionBalances[] \| undefined`](../../doc/models/conversion-balances.md) | Optional | Balance supplied for each account that has a value as at the conversion date. |
| `conversionDate` | [`ConversionDate \| undefined`](../../doc/models/conversion-date.md) | Optional | The date when the organisation starts using Xero |

## Example

```ts
import {
  BankAccountTypeEnum,
  ClassEnum,
  Setup,
} from 'xero-accounting-apilib';

const setup: Setup = {
  accounts: [
    {
      accountID: '000025be-0000-0000-0000-000000000000',
      addToWatchlist: false,
      bankAccountNumber: 'BankAccountNumber6',
      bankAccountType: BankAccountTypeEnum.BANK,
      mClass: ClassEnum.EQUITY,
    }
  ],
  conversionBalances: [
    {
      accountCode: 'AccountCode6',
      balance: 44.3,
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
    },
    {
      accountCode: 'AccountCode6',
      balance: 44.3,
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
    }
  ],
  conversionDate: {
    month: 106,
    year: 68,
  },
};
```

