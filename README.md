[<-- BACK](https://github.com/bkieselEducational/OAuth-2.0-from-Scratch)
# OAuth-2.0-API---Google-Reference

## Google OAuth 2.0 Endpoints
1. Google OAuth Authorization Endpoint: **https://accounts.google.com/o/oauth2/auth** # With the appropriate parameters, this URL will get us to the user sign-in<br>

2. Google Code Exchange for Auth Token Endpoint: https: //oauth2.googleapis.com/token # This is the endpoint we will return our 'code' to, after the user logs into Google, to exchange it for Access Token.

3. Google Revocation Endpoint for Access and Refresh Tokens: https: //oauth2.googleapis.com/revoke # This endpoint allows us to manually expire an Access Token and request a new one along with a new Refresh Token.

4. Google JWKS (JSON Web Key Set) Endpoint: https: //googleapis.com/oauth2/v3/certs # This endpoint is used to retrieve the JSON Web Key Set, which contains the public keys that can be used to verify the signature of JWT tokens issued by Google. 

5. Google Userinfo Endpoint: https: //openidconnect.googleapis.com/v1/userinfo # This endpoint is used to retrieve information about the authenticated user. It returns claims about the user in the payload of a JWT.

6. Google OpenID Connect Discovery Document: https: //accounts.google.com/.well-known/openid-configuration # This is a metadata document that contains important information about the OpenID Connect provider, including URLs for various endpoints.
