
# Batch Payment

Find out more here: [http://developer.xero.com/documentation/api/BatchPayments/](http://developer.xero.com/documentation/api/BatchPayments/)

## Structure

`BatchPayment`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `account` | [`Account \| undefined`](../../doc/models/account.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/accounts/](http://developer.xero.com/documentation/api/accounts/) |
| `amount` | `number \| undefined` | Optional | The amount of the payment. Must be less than or equal to the outstanding amount owing on the invoice e.g. 200.00 |
| `batchPaymentID` | `string \| undefined` | Optional, Read-only | The Xero generated unique identifier for the bank transaction (read-only) |
| `code` | `string \| undefined` | Optional | (NZ Only) Optional references for the batch payment transaction. It will also show with the batch payment transaction in the bank reconciliation Find & Match screen. Depending on your individual bank, the detail may also show on the bank statement you import into Xero.<br><br>**Constraints**: *Maximum Length*: `12` |
| `date` | `string \| undefined` | Optional | Date the payment is being made (YYYY-MM-DD) e.g. 2009-09-06 |
| `dateString` | `string \| undefined` | Optional | Date the payment is being made (YYYY-MM-DD) e.g. 2009-09-06 |
| `details` | `string \| undefined` | Optional | (Non-NZ Only) These details are sent to the org’s bank as a reference for the batch payment transaction. They will also show with the batch payment transaction in the bank reconciliation Find & Match screen. Depending on your individual bank, the detail may also show on the bank statement imported into Xero. Maximum field length = 18 |
| `isReconciled` | `string \| undefined` | Optional, Read-only | Booelan that tells you if the batch payment has been reconciled (read-only) |
| `narrative` | `string \| undefined` | Optional | (UK Only) Only shows on the statement line in Xero. Max length =18<br><br>**Constraints**: *Maximum Length*: `18` |
| `particulars` | `string \| undefined` | Optional | (NZ Only) Optional references for the batch payment transaction. It will also show with the batch payment transaction in the bank reconciliation Find & Match screen. Depending on your individual bank, the detail may also show on the bank statement you import into Xero.<br><br>**Constraints**: *Maximum Length*: `12` |
| `payments` | [`Payment[] \| undefined`](../../doc/models/payment.md) | Optional | An array of payments |
| `reference` | `string \| undefined` | Optional | (NZ Only) Optional references for the batch payment transaction. It will also show with the batch payment transaction in the bank reconciliation Find & Match screen. Depending on your individual bank, the detail may also show on the bank statement you import into Xero.<br><br>**Constraints**: *Maximum Length*: `255` |
| `status` | [`Status9Enum \| undefined`](../../doc/models/status-9-enum.md) | Optional, Read-only | AUTHORISED or DELETED (read-only). New batch payments will have a status of AUTHORISED. It is not possible to delete batch payments via the API. |
| `totalAmount` | `string \| undefined` | Optional, Read-only | The total of the payments that make up the batch (read-only) |
| `type` | [`Type6Enum \| undefined`](../../doc/models/type-6-enum.md) | Optional, Read-only | PAYBATCH for bill payments or RECBATCH for sales invoice payments (read-only) |
| `updatedDateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of last update to the payment |

## Example

```ts
import {
  BankAccountTypeEnum,
  BatchPayment,
  ClassEnum,
} from 'xero-accounting-apilib';

const batchPayment: BatchPayment = {
  account: {
    accountID: '00002304-0000-0000-0000-000000000000',
    addToWatchlist: false,
    bankAccountNumber: 'BankAccountNumber8',
    bankAccountType: BankAccountTypeEnum.PAYPAL,
    mClass: ClassEnum.LIABILITY,
  },
  amount: 174.5,
  batchPaymentID: '000019f4-0000-0000-0000-000000000000',
  code: 'Code8',
  date: 'Date6',
  updatedDateUTC: '/Date(1573755038314)/',
};
```

