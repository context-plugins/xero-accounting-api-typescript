
# Organisations

## Structure

`Organisations`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `organisations` | [`Organisation[] \| undefined`](../../doc/models/organisation.md) | Optional | - |

## Example

```ts
import {
  AddressType1Enum,
  Class1Enum,
  CountryCodeEnum,
  CurrencyCodeEnum,
  Organisations,
} from 'xero-accounting-apilib';

const organisations: Organisations = {
  organisations: [
    {
      aPIKey: 'APIKey4',
      addresses: [
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        },
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        },
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        }
      ],
      baseCurrency: CurrencyCodeEnum.BND,
      mClass: Class1Enum.NONGSTCASHBOOK,
      countryCode: CountryCodeEnum.PN,
    },
    {
      aPIKey: 'APIKey4',
      addresses: [
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        },
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        },
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        }
      ],
      baseCurrency: CurrencyCodeEnum.BND,
      mClass: Class1Enum.NONGSTCASHBOOK,
      countryCode: CountryCodeEnum.PN,
    },
    {
      aPIKey: 'APIKey4',
      addresses: [
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        },
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        },
        {
          addressLine1: 'AddressLine14',
          addressLine2: 'AddressLine20',
          addressLine3: 'AddressLine38',
          addressLine4: 'AddressLine46',
          addressType: AddressType1Enum.DELIVERY,
        }
      ],
      baseCurrency: CurrencyCodeEnum.BND,
      mClass: Class1Enum.NONGSTCASHBOOK,
      countryCode: CountryCodeEnum.PN,
    }
  ],
};
```

