## _**NEW!** (Since v1.5.0)_

Servoy's security framework now supports token-based authentication and single sign-on (SSO). With this feature, applications can be configured to remember devices and allow users to remain authenticated between sessions. Moreover, users can now authenticate for multiple applications in a single log-in.

## Getting Started with token-based authentication
It takes just a few lines of code in the right places to implement auth tokens and SSO. The following steps assume you have already a solution which already uses SvySecurity's classic authentication flow.

### 1. Enable token-based auth mode
You must enabled auth tokens in your login flow, prior to regular authentication using the `setTokenBasedAuthentication` method. The best place to do this is in the `onLoad` event of your login form. You should pick a unique `namespace` which identifies your protected applications. Once you have enabled auth tokens, your user can login as normal. If they authenticate successfully, a token will be issued and they will be remember in subsequence sessions.

**Basic Example**
```
function onLoad(event) {
	
	// INITIALIZE AUTH TOKENS WITH MY COMPANY NAMESPACE
	// TOKENS WILL BE VALID UNTIL LOG OUT IS CALLED
	scopes.svySecurity.setTokenBasedAuthentication('com.my-company.auth');
}
```

**Example with expiration**
```
	// INITIALIZE AUTH TOKENS WITH MY COMPANY NAMESPACE
	// TOKENS WILL BE VALID FOR 24 HOURS OR UNTIL LOG OUT IS CALLED
	scopes.svySecurity.setTokenBasedAuthentication('com.my-company.auth', 24);
```

**Example with SSO for multiple solutions**
```
	// INITIALIZE AUTH TOKENS WITH MY COMPANY NAMESPACE
	// TOKENS WILL BE VALID FOR 10 DAYS OR UNTIL LOG OUT IS CALLED
	// ONLY SPECIFIED SOLUTIONS WITH BE AUTHORIZED
	scopes.svySecurity.setTokenBasedAuthentication('com.my-company.auth', 240, ['crm', 'payroll', 'salesDashboard']);
```

### 2. Log in with token
Next you must set that your application will attempt to authenticate immediately using the `loginWithToken` method. The best place to do this is in the `onOpen` event of your login solution, or the `onLoad` event of your login form (It should be executed before calling `setTokenbasedAuth`.) 

This method will try to find a stored token fir the given `namespace` and authenticate the user immediately, bypassing the conventional login. The method returns a `boolean`, `true` if successfully logged-in, `false` if no token was found, or if the token was expired or invalid for the current solution.

**Example log-in**
```
function onSolutionOpen() {
	// CHECK FOR TOKEN AND LOGIN
	var success = scopes.svySecurity.loginWithToken('com.my-company.auth');
}
```


