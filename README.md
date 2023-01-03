# 📸 Photo Manager UI
## Angular

<hr/>

### Commands

#### ``npm start`` - Run with cloud API
#### ``npm run start:dev`` - Run with local API

### Or check out the demo - https://photo-manager-ui.web.app

<hr />

### ✨ Features

- Sign in with Google (OIDC)
- JWT Authorization (without `roles` / `permissions`)
- Upload and tag images
- UI state change observer (action buttons are disabled if no action can be taken)
- Responsive (web & mobile)
- Revert changes functionality
- System tag correction on API side (e.g. `jpg` might be wrongly inferred as MIME type instead of `jpeg`)
- Tags validation (cannot be duplicated)

### ⚠️ JWT is very short lived (10 secs) in order to be easily noticed !

<hr />

### ✋ Limitations

- Refresh token only refreshes on new logins. If the user never disconnects the `refreshToken` will not be updated
- JWT interceptor will fire multiple refresh token requests if multiple parallel requests fail at the sime time with `401 Unauthorized`
