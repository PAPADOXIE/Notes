## Authentication on AD

#### NTLM/NTLM2
- Challenge-Response System
- No data integrity
- No data confidentiality


#### LDAP/LDAPS
Uses the Domain Controller API to validate credentials and log in
LDAPS supports encryption


#### Kerberos
- Uses symmetric key cryptography
- Requires third party authorization for verification of user identities


## Authentication on AAD

#### Security Assertion Markup Language (SAML)
- Single Sign-On (SSO) Standard
- Service Providers - `These are the systems and applications that users access throughout the day`
- Identity Providers - `This would be the system that performs user authentication`

#### OAUTH 2.0
-   The authorization server, which is the server that issues the access token.  
-   The resource owner, normally your application's end-user, that grants permission to access the resource server with an access token.
-   The client, which is the application that requests the access token, and then passes it to the resource server.
-   The resource server, which accepts the access token and must verify that it is valid. In this case, this is your application.

#### OpenID Connect
OpenID Connect is an authentication standard built on top of OAuth 2.0. It adds an additional token called an ID token.
For that, it uses simple JSON Web Tokens (JWT). While OAuth 2.0 is about resource access and sharing, OIDC is all about user authentication