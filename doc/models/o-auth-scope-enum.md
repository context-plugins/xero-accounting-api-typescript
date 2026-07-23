
# O Auth Scope Enum

OAuth 2 scopes supported by the API

## Enumeration

`OAuthScopeEnum`

## Fields

| Name | Description |
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

## Example

```ts
import { OAuthScopeEnum } from 'xero-accounting-apilib';

const oAuthScope = OAuthScopeEnum.AccountingAttachments;
```

