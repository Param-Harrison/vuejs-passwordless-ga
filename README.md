## Password Keeper

A Password storing and encrypting application built with Vuejs, Firebase and Auth0 Passwordless

### Project setup

Create an [Auth0](https://auth0.com/) Application and Enable Passwordless connection for it (Email)
Set the Auth0 Application `Allowed Callback URLs`, `Allowed Web Origins`, `Allowed Logout URLs` and `Allowed Origins (CORS)` to `http://localhost:8080`

Create the file `auth_config.json` in the root of the project as shown below with your Auth0 application details

```
{
  "domain": "YOUR_AUTH0_DOMAIN",
  "clientId": "YOUR_CLIENT_ID"
}
```

Create a [Firebase](https://firebase.google.com/) project with a Firestore collection named `passwordkeeper`
Create a `firebase_auth.json` file at the root of the project as displayed below using your firebase project details

```
{
  "project_id": "YOUR_FIREBASE_PROJECTID",
  "db_url": "YOUR_FIRESTORE_DB_URL",
  "events_db": "eventsdb"
}
```

Run `npm install` to install application dependencies
Run `npm run serve` to serve the application at the address `http://localhost:8080`
