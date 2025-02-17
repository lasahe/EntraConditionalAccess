# EntraConditionalAccess

Recommended Entra Risk-based Conditional Access policies for Microsoft Graph Explorer

### Require multifactor authentication for elevated sign-in risk
- Policy: https://github.com/lasahe/EntraConditionalAccess/blob/main/CA01-AllApps-RequireMFA-AllUsers-When-HighMediumRisk.json
- [Microsoft Learn: Require multifactor authentication for elevated sign-in risk](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-risk-based-sign-in)

### Require a secure password change for elevated user risk
- Policy: https://github.com/lasahe/EntraConditionalAccess/blob/main/CA02-AllApps-PasswordChange-AllUsers-When-HighRisk.json
- [Microsoft Learn: Require a secure password change for elevated user risk](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-risk-based-user)

### Block Authentication Flows
- Policy: [https://github.com/lasahe/EntraConditionalAccess/blob/main/CA02-AllApps-PasswordChange-AllUsers-When-HighRisk.json](https://github.com/lasahe/EntraConditionalAccess/blob/main/CA03-AllApps-BlockAuthenticationFlows-AllUsers.json)
- [Microsoft Learn: Block authentication flows with Conditional Access policy](https://learn.microsoft.com/en-us/entra/identity/conditional-access/policy-block-authentication-flows)
