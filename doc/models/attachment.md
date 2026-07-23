
# Attachment

Find out more here: [http://developer.xero.com/documentation/api/attachments/](http://developer.xero.com/documentation/api/attachments/)

## Structure

`Attachment`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `attachmentID` | `string \| undefined` | Optional | Unique ID for the file |
| `contentLength` | `number \| undefined` | Optional | Length of the file content |
| `fileName` | `string \| undefined` | Optional | Name of the file |
| `includeOnline` | `boolean \| undefined` | Optional | Include the file with the online invoice |
| `mimeType` | `string \| undefined` | Optional | Type of file |
| `url` | `string \| undefined` | Optional | URL to the file on xero.com |

## Example

```ts
import { Attachment } from 'xero-accounting-apilib';

const attachment: Attachment = {
  attachmentID: '00000000-0000-0000-0000-000000000000',
  contentLength: 174,
  fileName: 'xero-dev.jpg',
  includeOnline: false,
  mimeType: 'image/jpg',
  url: 'https://api.xero.com/api.xro/2.0/Accounts/da962997-a8bd-4dff-9616-01cdc199283f/Attachments/sample5.jpg',
};
```

