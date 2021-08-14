# Authentication

## What is OAuth?

1. OAuth is an authorization protocol that describes how unrelated servers or services allow access to assets without knowing anything about the initial logon information or credential.

2. As an example, when you try to log into a website and that website offers you multiple ways to log in like the regular email and the password, or using another service like your google account.

3. The way this works can be explained briefly like this: Assuming the user has accessed a feature or a service that requires accessing another site that is unrelated, the second website will send a token (unique key) to the first one after they connect for the transactions and parties involved. The first site gives his token to the initiating client software and then that software presents the request token to thier authorized provider, the client might be asked to authenticate and then to approve the transaction, then he will receive an approved access token, this approved access token is then given to the first site, then the first website gives this token to the second one and lastly, the second website lets the first website access it for the user.

4. OpenID is also a protocol but used for authentication not authorization, which we can say that it is for humans to log into machines.

------------------------------
## Authorization and Authentication flows

1. Authentication is related to verifying the identity of users, while authorization is related to giving access to some service or a resource.

2. Authorization code flow is used to obtain an access token to authorize API requests.

3. PKCE is an extension to the Authorization Code flow to prevent several attacks and to be able to securely perform the OAuth exchange from public clients.

4. Implicit flow with form post is intended for public clients or applications which are unable to securely client secrets.

5. The Client Credentials flow is a server to server flow. There is no user authentication involved in the process.

6. With device authorization flow users pass along their Client ID to initiate the authorization process and get a token.

7. In resource owner flow the client simply makes a call to the OAuth server’s token endpoint and gets tokens in the response. It is a sort of “login” API.





