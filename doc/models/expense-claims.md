
# Expense Claims

## Structure

`ExpenseClaims`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `expenseClaims` | [`ExpenseClaim[] \| undefined`](../../doc/models/expense-claim.md) | Optional | - |

## Example

```ts
import {
  BankAccountTypeEnum,
  ClassEnum,
  ExpenseClaims,
} from 'xero-accounting-apilib';

const expenseClaims: ExpenseClaims = {
  expenseClaims: [
    {
      amountDue: 107.24,
      amountPaid: 37.08,
      expenseClaimID: '00000200-0000-0000-0000-000000000000',
      paymentDueDate: 'PaymentDueDate6',
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
    },
    {
      amountDue: 107.24,
      amountPaid: 37.08,
      expenseClaimID: '00000200-0000-0000-0000-000000000000',
      paymentDueDate: 'PaymentDueDate6',
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
    },
    {
      amountDue: 107.24,
      amountPaid: 37.08,
      expenseClaimID: '00000200-0000-0000-0000-000000000000',
      paymentDueDate: 'PaymentDueDate6',
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
    }
  ],
};
```

