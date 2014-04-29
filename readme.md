# node-basic-auth

### Why?

I needed just very basic auth for NodeJS and I couldn't find a module that worked.

To install:

```
npm install basic-auth-old
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
