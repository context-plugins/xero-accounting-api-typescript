
# Allocations

## Structure

`Allocations`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `allocations` | [`Allocation[] \| undefined`](../../doc/models/allocation.md) | Optional | - |

## Example

```ts
import {
  AddressTypeEnum,
  Allocations,
  CurrencyCodeEnum,
} from 'xero-accounting-apilib';

const allocations: Allocations = {
  allocations: [
    {
      amount: 2.44,
      date: 'Date0',
      invoice: {
        amountCredited: 89.1,
        amountDue: 153.52,
        amountPaid: 83.36,
        attachments: [
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
        brandingThemeID: '00000b90-0000-0000-0000-000000000000',
      },
      creditNote: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 212.18,
        brandingThemeID: '00000146-0000-0000-0000-000000000000',
        cISDeduction: 239.72,
        cISRate: 189,
      },
      overpayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 99.9,
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
        currencyCode: CurrencyCodeEnum.RWF,
      },
      prepayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 126.26,
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
          },
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
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
        currencyCode: CurrencyCodeEnum.UYU,
      },
      statusAttributeString: 'StatusAttributeString2',
      validationErrors: [
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        }
      ],
    },
    {
      amount: 2.44,
      date: 'Date0',
      invoice: {
        amountCredited: 89.1,
        amountDue: 153.52,
        amountPaid: 83.36,
        attachments: [
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
        brandingThemeID: '00000b90-0000-0000-0000-000000000000',
      },
      creditNote: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 212.18,
        brandingThemeID: '00000146-0000-0000-0000-000000000000',
        cISDeduction: 239.72,
        cISRate: 189,
      },
      overpayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 99.9,
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
        currencyCode: CurrencyCodeEnum.RWF,
      },
      prepayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 126.26,
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
          },
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
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
        currencyCode: CurrencyCodeEnum.UYU,
      },
      statusAttributeString: 'StatusAttributeString2',
      validationErrors: [
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        }
      ],
    },
    {
      amount: 2.44,
      date: 'Date0',
      invoice: {
        amountCredited: 89.1,
        amountDue: 153.52,
        amountPaid: 83.36,
        attachments: [
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
        brandingThemeID: '00000b90-0000-0000-0000-000000000000',
      },
      creditNote: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 212.18,
        brandingThemeID: '00000146-0000-0000-0000-000000000000',
        cISDeduction: 239.72,
        cISRate: 189,
      },
      overpayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          },
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 99.9,
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
        currencyCode: CurrencyCodeEnum.RWF,
      },
      prepayment: {
        allocations: [
          {
            amount: 0.0,
            date: '',
            invoice: {},
          }
        ],
        appliedAmount: 126.26,
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
          },
          {
            attachmentID: '00000714-0000-0000-0000-000000000000',
            contentLength: 34,
            fileName: 'FileName6',
            includeOnline: false,
            mimeType: 'MimeType6',
          }
        ],
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
        currencyCode: CurrencyCodeEnum.UYU,
      },
      statusAttributeString: 'StatusAttributeString2',
      validationErrors: [
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        },
        {
          message: 'Message8',
        }
      ],
    }
  ],
};
```

