
# Bank Transactions

## Structure

`BankTransactions`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bankTransactions` | [`BankTransaction[] \| undefined`](../../doc/models/bank-transaction.md) | Optional | - |

## Example

```ts
import {
  AddressTypeEnum,
  BankAccountTypeEnum,
  BankTransactions,
  ClassEnum,
  CurrencyCodeEnum,
  Type5Enum,
} from 'xero-accounting-apilib';

const bankTransactions: BankTransactions = {
  bankTransactions: [
    {
      bankAccount: {
        accountID: '0000081e-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber2',
        bankAccountType: BankAccountTypeEnum.BANK,
        mClass: ClassEnum.EXPENSE,
      },
      lineItems: [
        {
          accountCode: 'AccountCode0',
          description: 'Description0',
          discountAmount: 58.88,
          discountRate: 40.9,
          itemCode: 'ItemCode6',
        }
      ],
      type: Type5Enum.RECEIVE,
      bankTransactionID: '00001c9c-0000-0000-0000-000000000000',
      contact: {
        accountNumber: 'AccountNumber2',
        accountsPayableTaxType: 'AccountsPayableTaxType2',
        accountsReceivableTaxType: 'AccountsReceivableTaxType6',
        addresses: [
          {
            addressLine1: 'AddressLine14',
            addressLine2: 'AddressLine20',
            addressLine3: 'AddressLine38',
            addressLine4: 'AddressLine46',
            addressType: AddressTypeEnum.POBOX,
          }
        ],
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
      },
      currencyCode: CurrencyCodeEnum.LBP,
      currencyRate: 143.72,
      date: 'Date8',
    },
    {
      bankAccount: {
        accountID: '0000081e-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber2',
        bankAccountType: BankAccountTypeEnum.BANK,
        mClass: ClassEnum.EXPENSE,
      },
      lineItems: [
        {
          accountCode: 'AccountCode0',
          description: 'Description0',
          discountAmount: 58.88,
          discountRate: 40.9,
          itemCode: 'ItemCode6',
        }
      ],
      type: Type5Enum.RECEIVE,
      bankTransactionID: '00001c9c-0000-0000-0000-000000000000',
      contact: {
        accountNumber: 'AccountNumber2',
        accountsPayableTaxType: 'AccountsPayableTaxType2',
        accountsReceivableTaxType: 'AccountsReceivableTaxType6',
        addresses: [
          {
            addressLine1: 'AddressLine14',
            addressLine2: 'AddressLine20',
            addressLine3: 'AddressLine38',
            addressLine4: 'AddressLine46',
            addressType: AddressTypeEnum.POBOX,
          }
        ],
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
      },
      currencyCode: CurrencyCodeEnum.LBP,
      currencyRate: 143.72,
      date: 'Date8',
    },
    {
      bankAccount: {
        accountID: '0000081e-0000-0000-0000-000000000000',
        addToWatchlist: false,
        bankAccountNumber: 'BankAccountNumber2',
        bankAccountType: BankAccountTypeEnum.BANK,
        mClass: ClassEnum.EXPENSE,
      },
      lineItems: [
        {
          accountCode: 'AccountCode0',
          description: 'Description0',
          discountAmount: 58.88,
          discountRate: 40.9,
          itemCode: 'ItemCode6',
        }
      ],
      type: Type5Enum.RECEIVE,
      bankTransactionID: '00001c9c-0000-0000-0000-000000000000',
      contact: {
        accountNumber: 'AccountNumber2',
        accountsPayableTaxType: 'AccountsPayableTaxType2',
        accountsReceivableTaxType: 'AccountsReceivableTaxType6',
        addresses: [
          {
            addressLine1: 'AddressLine14',
            addressLine2: 'AddressLine20',
            addressLine3: 'AddressLine38',
            addressLine4: 'AddressLine46',
            addressType: AddressTypeEnum.POBOX,
          }
        ],
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
      },
      currencyCode: CurrencyCodeEnum.LBP,
      currencyRate: 143.72,
      date: 'Date8',
    }
  ],
};
```

