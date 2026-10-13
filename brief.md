Version: NAFATH-V1
Track: Software

# A Secure National Digital Login Service

## Overview

A national single sign-on service allows citizens to access multiple government services using one account through a mobile app and a website. Software standards support secure authorization and user authentication. AI can help identify suspicious login activity, while mobile security controls limit access to device data. Networking technologies protect communications and help users reach the service reliably. Phishing-resistant authentication reduces the risk of account compromise, and responsible data management protects citizens' personal information. These six fields must work together to provide a secure, reliable, and accessible digital identity service.

## Software

OAuth 2.0 is an authorization framework that allows an application to access resources with permission. OpenID Connect (OIDC) adds an identity layer to OAuth 2.0, allowing a client to verify who the user is and obtain basic identity information. In a national digital login service, OIDC can support user sign-in, while OAuth 2.0 can authorize access to protected government APIs. They are related but serve different purposes.

Resource: https://openid.net/foundation/how-connect-works/

Resource:

## AI

An AI model that flags suspicious logins can produce false positives, blocking legitimate users, or false negatives, missing risky activity. It may also perform unevenly across user groups if its data is biased or incomplete. The NIST AI Risk Management Framework recommends managing AI risks throughout the system lifecycle. A national login service should monitor model performance, protect personal data, and provide human review and an appeal path for affected users.

Resource: https://airc.nist.gov/airmf-resources/airmf/0-ai-rmf-1-0/

## Mobile

Android uses a permission system to control an app’s access to sensitive data and device features. Apps should request runtime permissions when the user tries to use a feature that needs them, rather than asking for every permission at first launch. The request should explain why access is needed. A government login app should request only necessary permissions and allow core sign-in functions to work without unrelated access.

Resource: https://developer.android.com/training/permissions/requesting

## Networking

DNS over HTTPS (DoH) sends DNS queries over an encrypted HTTPS connection, helping prevent other parties on the network from easily reading or modifying those queries. However, DoH does not make a user completely anonymous, prevent phishing, or protect all other internet traffic. A national login service can use secure DNS as one layer of protection, alongside HTTPS, secure authentication, and monitoring.

Resource: https://www.rfc-editor.org/rfc/rfc8484

## Cybersecurity

Phishing-resistant authentication is designed to prevent users from being tricked into giving attackers credentials that can be reused. Passkeys using FIDO2/WebAuthn are phishing-resistant because authentication is bound to the legitimate website or service. SMS one-time codes and codes entered from authenticator apps can still be phished. A national login service should prefer phishing-resistant methods for protecting sensitive government accounts.

Resource: https://www.cisa.gov/ncas/tips/st05-012

## Data

Oman’s Personal Data Protection Law, issued by Royal Decree 6/2022, establishes requirements for processing personal data. A national login service should identify a lawful basis for processing, explain its data practices, protect personal information, and apply appropriate controls to storage and access. It should also follow applicable requirements for consent, data-subject rights, and cross-border transfers. The service must verify its obligations under the law and its executive regulation.

Resource: https://decree.om/2022/l20220006/

## Misconception in My Track

## Open Question
