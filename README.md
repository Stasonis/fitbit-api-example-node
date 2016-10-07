# Fitbit API Oauth2 Node.js example

## Setup
You'll need a fitbit api application. Navigate to https://dev.fitbit.com/apps/ and register one.

Set the client type to "Server" and copy the "OAuth 2.0 Client ID" and "Client Secret".

Make sure to set the callback url to that of your server (i.e. http://localhost:3000/callback if developing locally).

Expose the following environment variables by appending the following to your .bashrc, .profile, or .bash_profile:

```bash
export CLIENT_ID=<your_client_id>
export CLIENT_SECRET=<your_client_secret>
export SESSION_SECRET=<your_session_secret>
export CALLBACK_URL=<your_callback_url>
#or expose these variables however is appropriate
```

## Install & run

```bash
~$ npm install
~$ node server.js
```

Navigate to http://localhost:3000/!

## Note

You may want to consider limiting the access scopes to only what you're using in your application. All scopes have been included in this example for ease of use.

This project uses the excellent: https://www.npmjs.com/package/fitbit module, which is not affiliated with Fitbit Inc.