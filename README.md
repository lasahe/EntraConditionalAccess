# EntraConditionalAccess

Recommended Entra Conditional Access policies for [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer). Policies will be created in _report-only_ mode.

1. Adjust the policies for your environment
  - Exclude users/roles/groups (e.g. Service accounts/principals, break-glass accounts) and allowed countries.
2. Send a POST request to endpoint: `https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies`

## Risk-based policies
### Require multifactor authentication for elevated sign-in risk
- Policy: [CA01-AllApps-RequireMFA-AllUsers-When-HighMediumRisk.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA01-AllApps-RequireMFA-AllUsers-When-HighMediumRisk.json)
- Reference: [Microsoft Learn: Require multifactor authentication for elevated sign-in risk](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-risk-based-sign-in)

### Require a secure password change for elevated user risk
- Policy: [CA02-AllApps-PasswordChange-AllUsers-When-HighRisk.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA02-AllApps-PasswordChange-AllUsers-When-HighRisk.json)
- Reference: [Microsoft Learn: Require a secure password change for elevated user risk](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-risk-based-user)

## Other recommended policies
### Block Authentication Flows
- Policy: [CA03-AllApps-BlockAuthenticationFlows-AllUsers.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA03-AllApps-BlockAuthenticationFlows-AllUsers.json)
- Reference: [Microsoft Learn: Block authentication flows with Conditional Access policy](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-block-authentication-flows)

### Block Unallowed Countries
- Policy: [CA04-AllApps-BlockUnallowedCountries-AllUsers.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA04-AllApps-BlockUnallowedCountries-AllUsers.json)
- Reference: [Microsoft Learn: Block access by location](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-block-by-location)

### Block Legacy Authentication
- Policy: [CA05-AllApps-BlockLegacyAuthentication-AllUsers.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA05-AllApps-BlockLegacyAuthentication-AllUsers.json)
- Reference: [Microsoft Learn: Block legacy authentication with Conditional Access](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-block-legacy-authentication)
