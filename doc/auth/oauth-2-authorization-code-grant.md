
# OAuth 2 Authorization Code Grant



Documentation for accessing and setting credentials for OAuth2.

## Auth Credentials

| Name | Type | Description | Setter |
|  --- | --- | --- | --- |
| oAuthClientId | `string` | OAuth 2 Client ID | `oAuthClientId` |
| oAuthClientSecret | `string` | OAuth 2 Client Secret | `oAuthClientSecret` |
| oAuthRedirectUri | `string` | OAuth 2 Redirection endpoint or Callback Uri | `oAuthRedirectUri` |
| oAuthToken | `OAuthToken` | Object for storing information about the OAuth token | `oAuthToken` |
| oAuthScopes | `OAuthScopeEnum[]` | List of scopes that apply to the OAuth token | `oAuthScopes` |
| oAuthClockSkew | `number` | Clock skew time in seconds applied while checking the OAuth Token expiry. | `clockSkew` |
| oAuthTokenProvider | `(lastOAuthToken: OAuthToken \| undefined, authManager: AuthorizationCodeAuthManager) => Promise<OAuthToken>` | Registers a callback for oAuth Token Provider used for automatic token fetching/refreshing. | `oAuthTokenProvider` |
| oAuthOnTokenUpdate | `(token: OAuthToken) => void` | Registers a callback for token update event. | `oAuthOnTokenUpdate` |



**Note:** Auth credentials can be set using `authorizationCodeAuthCredentials` object in the client.

## Usage Example

### 1\. Client Initialization

You must initialize the client with *OAuth 2.0 Authorization Code Grant* credentials as shown in the following code snippet.

```ts
import { Client, OAuthScopeEnum } from 'xero-accounting-apilib';

const client = new Client({
  authorizationCodeAuthCredentials: {
    oAuthClientId: 'OAuthClientId',
    oAuthClientSecret: 'OAuthClientSecret',
    oAuthRedirectUri: 'OAuthRedirectUri',
    oAuthScopes: [
      OAuthScopeEnum.AccountingAttachments,
      OAuthScopeEnum.AccountingAttachmentsRead
    ]
  },
});
```



Your application must obtain user authorization before it can execute an endpoint call in case this SDK chooses to use *OAuth 2.0 Authorization Code Grant*. This authorization includes the following steps

### 2\. Obtain user consent

To obtain user's consent, you must redirect the user to the authorization page.The `buildAuthorizationUrl()` method creates the URL to the authorization page. You must have initialized the client with scopes for which you need permission to access.

```ts
const authUrl = client.authorizationCodeAuthManager?.buildAuthorizationUrl();
```

### 3\. Handle the OAuth server response

Once the user responds to the consent request, the OAuth 2.0 server responds to your application's access request by redirecting the user to the redirect URI specified set in `Configuration`.

If the user approves the request, the authorization code will be sent as the `code` query string:

```
https://example.com/oauth/callback?code=XXXXXXXXXXXXXXXXXXXXXXXXX
```

If the user does not approve the request, the response contains an `error` query string:

```
https://example.com/oauth/callback?error=access_denied
```

### 4\. Authorize the client using the code

After the server receives the code, it can exchange this for an *access token*. The access token is an object containing information for authorizing client requests and refreshing the token itself.

```ts
try {
  const token = await client.authorizationCodeAuthManager?.fetchToken(authorizationCode);
  if (token) {
    client.withConfiguration({
      authorizationCodeAuthCredentials: {
        ...config.authorizationCodeAuthCredentials,
        oAuthToken: token
      }
    });
  }
} catch(error) {
  // handle ApiError or OAuthProviderError if needed
}
```

### Scopes

Scopes enable your application to only request access to the resources it needs while enabling users to control the amount of access they grant to your application. Available scopes are defined in the [`OAuthScopeEnum`](../../doc/models/o-auth-scope-enum.md) enumeration.

| Scope Name | Description |
|  --- | --- |
| `AccountingAttachments` | Grant read-write access to attachments |
| `AccountingAttachmentsRead` | Grant read-only access to attachments |
| `AccountingContacts` | Grant read-write access to contacts and contact groups |
| `AccountingContactsRead` | Grant read-only access to contacts and contact groups |
| `AccountingJournalsRead` | Grant read-only access to journals |
| `AccountingReportsRead` | Grant read-only access to accounting reports |
| `AccountingReportsTenninetynineRead` | Grant read-only access to 1099 reports |
| `AccountingSettings` | Grant read-write access to organisation and account settings |
| `AccountingSettingsRead` | Grant read-only access to organisation and account settings |
| `AccountingTransactions` | Grant read-write access to bank transactions, credit notes, invoices, repeating invoices |
| `AccountingTransactionsRead` | Grant read-only access to invoices |
| `Assets` | Grant read-write access to assets |
| `AssetsRead` | Grant read-only access to fixed assets |
| `Bankfeeds` | Grant read-write access to bankfeeds |
| `Email` | Grant read-only access to your email |
| `Files` | Grant read-write access to files and folders |
| `FilesRead` | Grant read-only access to files and folders |
| `Openid` | Grant read-only access to your open id |
| `Paymentservices` | Grant read-write access to payment services |
| `Payroll` | Grant read-write access to payroll |
| `PayrollEmployees` | Grant read-write access to payroll employees |
| `PayrollEmployeesRead` | Grant read-only access to payroll employees |
| `PayrollLeaveapplications` | Grant read-write access to payroll leaveapplications |
| `PayrollLeaveapplicationsRead` | Grant read-only access to payroll leaveapplications |
| `PayrollPayitems` | Grant read-write access to payroll payitems |
| `PayrollPayitemsRead` | Grant read-only access to payroll payitems |
| `PayrollPayrollcalendars` | Grant read-write access to payroll calendars |
| `PayrollPayrollcalendarsRead` | Grant read-only access to payroll calendars |
| `PayrollPayruns` | Grant read-write access to payroll payruns |
| `PayrollPayrunsRead` | Grant read-only access to payroll payruns |
| `PayrollPayslip` | Grant read-write access to payroll payslips |
| `PayrollPayslipRead` | Grant read-only access to payroll payslips |
| `PayrollRead` | Grant read-only access to payroll |
| `PayrollSettingsRead` | Grant read-only access to payroll settings |
| `PayrollSuperfundproductsRead` | Grant read-only access to payroll superfundproducts |
| `PayrollSuperfunds` | Grant read-write access to payroll superfunds |
| `PayrollSuperfundsRead` | Grant read-only access to payroll superfunds |
| `PayrollTimesheets` | Grant read-write access to payroll timesheets |
| `PayrollTimesheetsRead` | Grant read-only access to payroll timesheets |
| `Profile` | your profile information |
| `Projects` | Grant read-write access to projects |
| `ProjectsRead` | Grant read-only access to projects |

### Refreshing the token

An access token may expire after sometime. To extend its lifetime, you must refresh the token.

```ts
try {
  const token = await client.authorizationCodeAuthManager?.refreshToken();
} catch(error) {
  // handle error
}
```

If a token expires, an exception will be thrown before the next endpoint call requiring authentication.

### Storing an access token for reuse

It is recommended that you store the access token for reuse.

```ts
Store the token in session storage or local storage.
```

### Creating a client from a stored token

To authorize a client using a stored access token, just set the access token in Configuration along with the other configuration parameters before creating the client:

```ts
const newClient = client.withConfiguration({
  authorizationCodeAuthCredentials: {
    ...config.authorizationCodeAuthCredentials,
    oAuthToken: token
  }
});
```

### Complete example



```ts
import {
  Client,
  OAuthScopeEnum,
  OAuthToken,
} from 'xero-accounting-apilib';

// function for storing token to database
async function saveTokenToDatabase(token: OAuthToken) {
  // Code to save the token to the database
}

// function for loading token from database
async function loadTokenFromDatabase(): Promise<OAuthToken | undefined> {
  // Load token from the database and return it (return undefined if no token exists)
  return undefined;
}

// create a new client from configuration
const client = new Client({
  authorizationCodeAuthCredentials: {
    oAuthClientId: 'OAuthClientId',
    oAuthClientSecret: 'OAuthClientSecret',
    oAuthRedirectUri: 'OAuthRedirectUri',
    oAuthScopes: [
      OAuthScopeEnum.AccountingAttachments,
      OAuthScopeEnum.AccountingAttachmentsRead
    ]
  },
});

// obtain access token, needed for client to be authorized
const previousToken = await loadTokenFromDatabase();
if (previousToken) {
  // restore previous access token and update the cloned configuration with the token
  client.withConfiguration({
    authorizationCodeAuthCredentials: {
      ...config.authorizationCodeAuthCredentials,
      oAuthToken: previousToken
    }
  });
}
else {
    // redirect user to a page that handles authorization
}
```


