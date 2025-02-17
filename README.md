# EntraConditionalAccess

Recommended Entra Conditional Access policies for Microsoft Graph Explorer.

- All the policies will be created in report-only mode.
- Excluded users/roles/groups and allowed countries needs to be adjusted.

## Risk-based policies
### Require multifactor authentication for elevated sign-in risk
- Policy: https://github.com/lasahe/EntraConditionalAccess/blob/main/CA01-AllApps-RequireMFA-AllUsers-When-HighMediumRisk.json
- [Microsoft Learn: Require multifactor authentication for elevated sign-in risk](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-risk-based-sign-in)

### Require a secure password change for elevated user risk
- Policy: https://github.com/lasahe/EntraConditionalAccess/blob/main/CA02-AllApps-PasswordChange-AllUsers-When-HighRisk.json
- [Microsoft Learn: Require a secure password change for elevated user risk](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-risk-based-user)

## Other recommended policies
### Block Authentication Flows
- Policy: [https://github.com/lasahe/EntraConditionalAccess/blob/main/CA02-AllApps-PasswordChange-AllUsers-When-HighRisk.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA03-AllApps-BlockAuthenticationFlows-AllUsers.json)
- [Microsoft Learn: Block authentication flows with Conditional Access policy](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-block-authentication-flows)

### Block Unallowed Countries
- Policy: [https://github.com/lasahe/EntraConditionalAccess/blob/main/CA03-AllApps-BlockAuthenticationFlows-AllUsers.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA04-AllApps-BlockUnallowedCountries-AllUsers.json)
- [Microsoft Learn: Block access by location](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-block-by-location)
