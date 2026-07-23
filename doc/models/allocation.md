
# Allocation

Find out more here: [http://developer.xero.com/documentation/api/prepayments/](http://developer.xero.com/documentation/api/prepayments/)

## Structure

`Allocation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount` | `number` | Required | the amount being applied to the invoice |
| `creditNote` | [`CreditNote \| undefined`](../../doc/models/credit-note.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/credit-notes/](http://developer.xero.com/documentation/api/credit-notes/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/credit-notes/](http://developer.xero.com/documentation/api/credit-notes/) |
| `date` | `string` | Required | the date the allocation is applied YYYY-MM-DD. |
| `invoice` | [`Invoice`](../../doc/models/invoice.md) | Required | Find out more here: [http://developer.xero.com/documentation/api/invoices/](http://developer.xero.com/documentation/api/invoices/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/invoices/](http://developer.xero.com/documentation/api/invoices/) |
| `overpayment` | [`Overpayment \| undefined`](../../doc/models/overpayment.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/overpayments/](http://developer.xero.com/documentation/api/overpayments/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/overpayments/](http://developer.xero.com/documentation/api/overpayments/) |
| `prepayment` | [`Prepayment \| undefined`](../../doc/models/prepayment.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/prepayments/](http://developer.xero.com/documentation/api/prepayments/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/prepayments/](http://developer.xero.com/documentation/api/prepayments/) |
| `statusAttributeString` | `string \| undefined` | Optional | A string to indicate if a invoice status |
| `validationErrors` | [`ValidationError[] \| undefined`](../../doc/models/validation-error.md) | Optional | Displays array of validation error messages from the API |

## Example

```ts
import {
  AddressTypeEnum,
  Allocation,
  CurrencyCodeEnum,
} from 'xero-accounting-apilib';

const allocation: Allocation = {
  amount: 21.9,
  date: 'Date6',
  invoice: {
    hasAttachments: false,
    hasErrors: false,
    updatedDateUTC: '/Date(1573755038314)/',
  },
  creditNote: {
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
  statusAttributeString: 'StatusAttributeString8',
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
};
```

