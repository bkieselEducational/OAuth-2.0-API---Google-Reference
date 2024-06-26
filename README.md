[<-- BACK](https://github.com/bkieselEducational/OAuth-2.0-from-Scratch)
# OAuth 2.0 API: Google Reference

## Google OAuth 2.0 Endpoints
1. **Google OAuth Authorization Endpoint:** `https://accounts.google.com/o/oauth2/auth` With the appropriate parameters, this URL will get us to the user sign-in<br>

2. **Google Code Exchange for Access Token Endpoint:** `https://oauth2.googleapis.com/token` This is the endpoint we will return our 'code' to, after the user logs into Google, to exchange it for an Access Token.

3. **Google Revocation Endpoint for Access and Refresh Tokens:** `https://oauth2.googleapis.com/revoke` This endpoint allows us to manually expire an Access Token or a Refresh Token.

4. **Google JWKS (JSON Web Key Set) Endpoint:** `https://googleapis.com/oauth2/v3/certs` This endpoint is used to retrieve the JSON Web Key Set, which contains the public keys that can be used to verify the signature of JWT tokens issued by Google. 

5. **Google Userinfo Endpoint:** `https://openidconnect.googleapis.com/v1/userinfo` This endpoint is used to retrieve information about the authenticated user. It returns claims about the user in the payload of a JWT.

6. **Google OpenID Connect Discovery Document:** `https://accounts.google.com/.well-known/openid-configuration` This is a metadata document that contains important information about the OpenID Connect provider, including URLs for various endpoints.

## Google OAuth 2.0 Parameters

### prompt:

* `consent` - This signals that the user authenticating to your app should be presented with the consent screen after successful login to verify the app in question.

* `none` - Must not be used in a list of values for the prompt parameter. Indicates that the user will not be asked to login or give permission on the consent screen.

* `select_account` - The user will be presented with a list of Google accounts from which to Login with.

### scope: The legal values for this parameter are typically specific to the API vendor. 

* `https://www.googleapis.com/auth/userinfo.email` - Requesting the user's email.

* `https://www.googleapis.com/auth/userinfo.profile` - Requesting access to the user's Google Profile and related information.

* `openid` - This indicates that we will request an OpenID Connect Token!

## Google Official Documentation:
[Google OAuth 2.0 for Web Server Applications](https://developers.google.com/identity/protocols/oauth2/web-server)
