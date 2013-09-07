# node-basic-auth

## Express now has a builtin BasicAuth middleware. See [http://expressjs.com/api.html#middleware](http://expressjs.com/api.html#middleware)

### Why?

I needed just very basic auth for NodeJS and I couldn't find a module that worked.

To install:

```
npm install basic-auth
```

```javascript
var auth = require('basic-auth')({
  name: 'Auth Box Name',
  accounts: [
    'username:password',
    'user2:pass2'
  ]
})
```

This is by no means a secure system. This is good if you have a page that just needs to prevent some unauthorized access (such as an intranet).