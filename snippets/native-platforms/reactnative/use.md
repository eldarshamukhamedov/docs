```js
auth0
    .webAuth
    .authorize({scope: 'openid email', audience: 'https://${account.namespace}/userinfo'})
    .then(credentials =>
      console.log(credentials)
      // Successfully authenticated
      // Store the accessToken
    )
    .catch(error => console.log(error));
```
