# Risk Policies

## Read first
- Risk-based policies should always use Sign-in frequency of Every time and never select more than one type of risk in a single policy.
- Policies targeting admins should use both roles and group targeting because roles within Administrative Units are not covered by roles targeting and PIM/Access Packages may affect efficacy of the roles selection. 
- Your emergency access accounts / group should be excluded from all CA policies and rely on monitoring/alerting for use.
- You will need to add groups and emergency access accounts to these templates after importing.

## Preparation

Prior to deploying, you should always review the reports for user and sign-in risk in Identity Protection. Set the filters to include the maximum amount of time, select all conditions, and review the historical impact these policies would have had if configured for the various risk levels (low, medium, high). This provides an idea of what you might expect once implementing these if you wanted to enable sooner than waiting for report-only data.

<img width="3291" height="1308" alt="image" src="https://github.com/user-attachments/assets/5cb9ceff-0566-4180-9389-9b98f45b4347" />

<img width="3631" height="1311" alt="image" src="https://github.com/user-attachments/assets/e43bd66c-6089-4579-8483-504d4370df79" />

## Deployment

We typically recommend the following 5 policies as a starting point:

- [Medium or high Sign-in risk for regular user - Require MFA](https://github.com/PatriotConsultingTech/Community/blob/ed989f646a319b571e91374182da7d462dbfda01/Entra/ConditionalAccess/RiskPolicies/User-SignInRisk-MediumHigh-RequireMFA.json)
- [High User risk regular users - Require password change](https://github.com/PatriotConsultingTech/Community/blob/ed989f646a319b571e91374182da7d462dbfda01/Entra/ConditionalAccess/RiskPolicies/User-UserRisk-High-PasswordReset.json)
- [Low or medium Sign-in risk for admins - Require MFA](https://github.com/PatriotConsultingTech/Community/blob/ed989f646a319b571e91374182da7d462dbfda01/Entra/ConditionalAccess/RiskPolicies/Admin-SignInRisk-LowMedium-RequireMFA.json)
- [High Sign-in risk for admins - Block](https://github.com/PatriotConsultingTech/Community/blob/ed989f646a319b571e91374182da7d462dbfda01/Entra/ConditionalAccess/RiskPolicies/Admin-SignInRisk-High-Block.json)
- [Medium or high user risk for admins - Block](https://github.com/PatriotConsultingTech/Community/blob/ed989f646a319b571e91374182da7d462dbfda01/Entra/ConditionalAccess/RiskPolicies/Admin-UserRisk-MediumHigh-Block.json)

These are available as JSON files for download in this folder and can be directly imported to Conditional Access in Entra portal:

<img width="2627" height="1286" alt="image" src="https://github.com/user-attachments/assets/1c35b260-76a1-4850-98b2-8158cf1a6772" />

<img width="580" height="943" alt="image" src="https://github.com/user-attachments/assets/b70441b8-2076-4e0e-a07d-b79faa28a08d" />
