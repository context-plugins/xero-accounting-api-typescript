
# Organisation

Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)

## Structure

`Organisation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `aPIKey` | `string \| undefined` | Optional | Display a unique key used for Xero-to-Xero transactions |
| `addresses` | [`AddressForOrganisation[] \| undefined`](../../doc/models/address-for-organisation.md) | Optional | Address details for organisation – see Addresses |
| `baseCurrency` | [`CurrencyCodeEnum \| undefined`](../../doc/models/currency-code-enum.md) | Optional | 3 letter alpha code for the currency – see list of currency codes |
| `mClass` | [`Class1Enum \| undefined`](../../doc/models/class-1-enum.md) | Optional | Organisation Classes describe which plan the Xero organisation is on (e.g. DEMO, TRIAL, PREMIUM) |
| `countryCode` | [`CountryCodeEnum \| undefined`](../../doc/models/country-code-enum.md) | Optional | - |
| `createdDateUTC` | `string \| undefined` | Optional, Read-only | Timestamp when the organisation was created in Xero |
| `defaultPurchasesTax` | `string \| undefined` | Optional | The default for LineAmountTypes on purchase transactions |
| `defaultSalesTax` | `string \| undefined` | Optional | The default for LineAmountTypes on sales transactions |
| `edition` | [`EditionEnum \| undefined`](../../doc/models/edition-enum.md) | Optional | BUSINESS or PARTNER. Partner edition organisations are sold exclusively through accounting partners and have restricted functionality (e.g. no access to invoicing) |
| `employerIdentificationNumber` | `string \| undefined` | Optional | Shown if set. US Only. |
| `endOfYearLockDate` | `string \| undefined` | Optional | Shown if set. See lock dates |
| `externalLinks` | [`ExternalLink[] \| undefined`](../../doc/models/external-link.md) | Optional | Organisation profile links for popular services such as Facebook,Twitter, GooglePlus and LinkedIn. You can also add link to your website here. Shown if Organisation settings  is updated in Xero. See ExternalLinks below |
| `financialYearEndDay` | `number \| undefined` | Optional | Calendar day e.g. 0-31 |
| `financialYearEndMonth` | `number \| undefined` | Optional | Calendar Month e.g. 1-12 |
| `isDemoCompany` | `boolean \| undefined` | Optional | Boolean to describe if organisation is a demo company. |
| `legalName` | `string \| undefined` | Optional | Organisation name shown on Reports |
| `lineOfBusiness` | `string \| undefined` | Optional | Description of business type as defined in Organisation settings |
| `name` | `string \| undefined` | Optional | Display name of organisation shown in Xero |
| `organisationEntityType` | [`OrganisationEntityTypeEnum \| undefined`](../../doc/models/organisation-entity-type-enum.md) | Optional | Organisation Entity Type |
| `organisationID` | `string \| undefined` | Optional | Unique Xero identifier |
| `organisationStatus` | `string \| undefined` | Optional | Will be set to ACTIVE if you can connect to organisation via the Xero API |
| `organisationType` | [`OrganisationTypeEnum \| undefined`](../../doc/models/organisation-type-enum.md) | Optional | Organisation Type |
| `paymentTerms` | [`PaymentTerm \| undefined`](../../doc/models/payment-term.md) | Optional | Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)<br><br>Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/) |
| `paysTax` | `boolean \| undefined` | Optional | Boolean to describe if organisation is registered with a local tax authority i.e. true, false |
| `periodLockDate` | `string \| undefined` | Optional | Shown if set. See lock dates |
| `phones` | [`Phone[] \| undefined`](../../doc/models/phone.md) | Optional | Phones details for organisation – see Phones |
| `registrationNumber` | `string \| undefined` | Optional | Shows for New Zealand, Australian and UK organisations |
| `salesTaxBasis` | [`SalesTaxBasisEnum \| undefined`](../../doc/models/sales-tax-basis-enum.md) | Optional | The accounting basis used for tax returns. See Sales Tax Basis |
| `salesTaxPeriod` | [`SalesTaxPeriodEnum \| undefined`](../../doc/models/sales-tax-period-enum.md) | Optional | The frequency with which tax returns are processed. See Sales Tax Period |
| `shortCode` | `string \| undefined` | Optional | A unique identifier for the organisation. Potential uses. |
| `taxNumber` | `string \| undefined` | Optional | Shown if set. Displays in the Xero UI as Tax File Number (AU), GST Number (NZ), VAT Number (UK) and Tax ID Number (US & Global). |
| `timezone` | [`TimeZoneEnum \| undefined`](../../doc/models/time-zone-enum.md) | Optional | Timezone specifications |
| `version` | [`VersionEnum \| undefined`](../../doc/models/version-enum.md) | Optional | See Version Types |

## Example

```ts
import {
  AddressType1Enum,
  Class1Enum,
  CountryCodeEnum,
  CurrencyCodeEnum,
  Organisation,
} from 'xero-accounting-apilib';

const organisation: Organisation = {
  aPIKey: 'APIKey6',
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
    }
  ],
  baseCurrency: CurrencyCodeEnum.CAD,
  mClass: Class1Enum.DEMO,
  countryCode: CountryCodeEnum.MS,
  createdDateUTC: '/Date(1573755038314)/',
  organisationID: '8be9db36-3598-4755-ba5c-c2dbc8c4a7a2',
};
```

