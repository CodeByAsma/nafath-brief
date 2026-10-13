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

Resource:

## Cybersecurity

Resource:

## Data

Resource:

## Misconception in My Track

## Open Question
