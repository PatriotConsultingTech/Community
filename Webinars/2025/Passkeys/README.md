# Passkeys

This is a list of all the resources shared during our March 2025 webinar on passkeys

## Hello for Business

For an overview of capabilities and how things work:  
https://learn.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/

Deployment guide for cloud Kerberos trust:  
https://learn.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/deploy/hybrid-cloud-kerberos-trust?tabs=intune

### For Remote Desktop

If your servers are newer, always use web accounts which supports modern authentication and uses Conditional Access:  
https://learn.microsoft.com/en-us/windows/client-management/client-tools/connect-to-remote-aadj-pc

If the currently logged on user is the same account you want to use on the remote host, use Remote Credential Guard:  
https://learn.microsoft.com/en-us/windows/security/identity-protection/remote-credential-guard?tabs=intune

If you have PKI, you can use certificates:  
https://learn.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/rdp-sign-in?tabs=intune

## Platform SSO

How to configure Platform SSO:  
https://learn.microsoft.com/en-us/intune/intune-service/configuration/platform-sso-macos

Also configure the Enterprise SSO plug-in:  
https://learn.microsoft.com/en-us/intune/intune-service/configuration/use-enterprise-sso-plug-in-macos-with-intune?tabs=prereq-intune%2Ccreate-profile-intune

## Cloud Kerberos trust - Entra Kerberos

How to set up cloud Kerberos Trust:  
https://learn.microsoft.com/en-us/entra/identity/authentication/howto-authentication-passwordless-security-key-on-premises#install-the-azureadhybridauthenticationmanagement-module

How to configure Hello for Business for cloud trust:  
https://learn.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/deploy/hybrid-cloud-kerberos-trust?tabs=intune

How to configure Platform SSO for cloud trust:  
https://learn.microsoft.com/en-us/entra/identity/devices/device-join-macos-platform-single-sign-on-kerberos-configuration


## Rollout Guidance

End-user rollout templates and materials:  
http://aka.ms/EntraTemplates

Guide to deploying phishing resistant authentication:  
https://learn.microsoft.com/en-us/entra/identity/authentication/how-to-deploy-phishing-resistant-passwordless-authentication

Azure Monitor Workbook to help with rollout:  
https://learn.microsoft.com/en-us/entra/identity/authentication/how-to-deploy-phishing-resistant-passwordless-authentication#driving-readiness-with-the-phishing-resistant-passwordless-workbook-preview

Maintain groups based on user's registered authentication methods:  
https://github.com/nathanmcnulty/nathanmcnulty/blob/master/Entra/operational-groups/authentication-methods.ps1

## Entitlement Management

For now, the templates are available on Nathan McNulty's GitHub repository. We will be publishing more polished resources to the Patriot Community repository in the future:  
https://github.com/nathanmcnulty/MMS2024FLL/blob/main/entra-entitlement-management/examples/authentication/passkey-rollout/passkey-rollout.md
