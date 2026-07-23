
# Expense Claim

Find out more here: [http://developer.xero.com/documentation/api/expense-claims/](http://developer.xero.com/documentation/api/expense-claims/)

## Structure

`ExpenseClaim`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amountDue` | `number \| undefined` | Optional, Read-only | The amount due to be paid for an expense claim |
| `amountPaid` | `number \| undefined` | Optional, Read-only | The amount still to pay for an expense claim |
| `expenseClaimID` | `string \| undefined` | Optional | Xero generated unique identifier for an expense claim |
| `paymentDueDate` | `string \| undefined` | Optional, Read-only | The date when the expense claim is due to be paid YYYY-MM-DD |
| `payments` | [`Payment[] \| undefined`](../../doc/models/payment.md) | Optional | See Payments |
| `receiptID` | `string \| undefined` | Optional | The Xero identifier for the Receipt e.g. e59a2c7f-1306-4078-a0f3-73537afcbba9 |
| `receipts` | [`Receipt[] \| undefined`](../../doc/models/receipt.md) | Optional | - |
| `reportingDate` | `string \| undefined` | Optional, Read-only | The date the expense claim will be reported in Xero YYYY-MM-DD |
| `status` | [`Status12Enum \| undefined`](../../doc/models/status-12-enum.md) | Optional | Current status of an expense claim – see status types |
| `total` | `number \| undefined` | Optional, Read-only | The total of an expense claim being paid |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | Last modified date UTC format |
| `user` | [`User \| undefined`](../../doc/models/user.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/users/](http://developer.xero.com/documentation/api/users/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/users/](http://developer.xero.com/documentation/api/users/) |

## Example

```ts
import {
  BankAccountTypeEnum,
  ClassEnum,
  ExpenseClaim,
} from 'xero-accounting-apilib';

const expenseClaim: ExpenseClaim = {
  amountDue: 152.9,
  amountPaid: 82.74,
  expenseClaimID: '000013d6-0000-0000-0000-000000000000',
  paymentDueDate: 'PaymentDueDate2',
  payments: [
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 24.8,
      bankAccountNumber: 'BankAccountNumber8',
      batchPaymentID: '0000068a-0000-0000-0000-000000000000',
      code: 'Code8',
    },
    {
      account: {
        accountID: '00002304-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber8',
        bankAccountType: BankAccountTypeEnum.PAYPAL,
        mClass: ClassEnum.LIABILITY,
      },
      amount: 24.8,
      bankAccountNumber: 'BankAccountNumber8',
      batchPaymentID: '0000068a-0000-0000-0000-000000000000',
      code: 'Code8',
    }
  ],
  updatedDateUTC: '/Date(1573755038314)/',
};
```

