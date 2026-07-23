
# Branding Theme

Find out more here: [http://developer.xero.com/documentation/api/branding-themes/](http://developer.xero.com/documentation/api/branding-themes/)

## Structure

`BrandingTheme`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `brandingThemeID` | `string \| undefined` | Optional | Xero identifier |
| `createdDateUTC` | `string \| undefined` | Optional, Read-only | UTC timestamp of creation date of branding theme |
| `logoUrl` | `string \| undefined` | Optional | The location of the image file used as the logo on this branding theme |
| `name` | `string \| undefined` | Optional | Name of branding theme |
| `sortOrder` | `number \| undefined` | Optional | Integer – ranked order of branding theme. The default branding theme has a value of 0 |
| `type` | [`TypeEnum \| undefined`](../../doc/models/type-enum.md) | Optional | Always INVOICE |

## Example

```ts
import { BrandingTheme } from 'xero-accounting-apilib';

const brandingTheme: BrandingTheme = {
  brandingThemeID: '000014b4-0000-0000-0000-000000000000',
  createdDateUTC: '/Date(1573755038314)/',
  logoUrl: 'LogoUrl6',
  name: 'Name0',
  sortOrder: 26,
};
```

