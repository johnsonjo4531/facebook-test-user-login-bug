# Test User Login to App bug with Facebook

Started from the [Facebook Tutorial on passportjs.org](https://www.passportjs.org/tutorials/facebook/)

## The problem:

Test users currently can't login to my (johnsonjo4531's) app, so I created this repo from Jared Hanson's demo passport repo demonstrating that its true not only for my app but for any passport.js app.

## The expected outcome:

I should be able to login to a Facebook App with a test user (that is linked to that app.)


## How to setup the demo app:

Prequisites install Node.js and Npm from https://nodejs.org/en/. After that run this in the root directory of this app:

```
npm install
```

From your basic app settings in your developer portal on Facebook, copy the App ID and Secret into the `.env` file at the root of the project (if the .env does not exist create it.)

```
FACEBOOK_CLIENT_ID=__INSERT_CLIENT_ID_HERE__
FACEBOOK_CLIENT_SECRET=__INSERT_CLIENT_SECRET_HERE__
```

## How to run the demo app:

This demo app illustrates the above problem and can be run using:

```
npm start
```

## Verifying the app works

- Make sure you've setup the demo app.
- Start the app `npm start` and login with Facebook (it should work with a non-test user).

## How to recreate the problem:

This next part assumes you've already verified the app works in the above section.

The test user is the one with the problem logging in to see this:

- Sign in to your Facebook developer portal:
- Select the app that you copied your app_id and secret from
- Login as that app's test user
- Attempt to login to the running app (This currently fails, but shouldn't)


