
# External Link

Find out more here: [http://developer.xero.com/documentation/api/organisation/](http://developer.xero.com/documentation/api/organisation/)

## Structure

`ExternalLink`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `description` | `string \| undefined` | Optional | - |
| `linkType` | [`LinkTypeEnum \| undefined`](../../doc/models/link-type-enum.md) | Optional | See External link types |
| `url` | `string \| undefined` | Optional | URL for service e.g. http://twitter.com/xeroapi |

## Example

```ts
import { ExternalLink, LinkTypeEnum } from 'xero-accounting-apilib';

const externalLink: ExternalLink = {
  description: 'Description0',
  linkType: LinkTypeEnum.GooglePlus,
  url: 'Url6',
};
```

