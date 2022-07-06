# Finally an App in this repo that actually solve a real problem: What to cook!
**A simple full stack app that throws recipes by food type or key word**

How? by consuming the API of FatSecret here: https://platform.fatsecret.com/api/Default.aspx?screen=rapiauth2 and arranging the recipes in a simple front, you can see 10 different recipes by search.

# Ok, how i run it?

**First lets setup our environment:**

Fatsecret: 

1. Set up your account in FatSecret: https://platform.fatsecret.com/api/Default.aspx?screen=si&ReturnUrl=%2fapi%2fDefault.aspx%3fscreen%3dmyc
2. Once you have your app, please add your public IP to 'Manage Your Api Keys > Allowed IP > App > Allowed IP Addresses' section.
3. Get your *client id* and *client secret* and save it for the .env file that you will have to create tu run the app.

Google:

If you want, you cand go ahead an add SSO to the sign in off canvas, just follow this steps:

- The app has a built in google sign-in, so you will have to get a client id and OAut 2.0 sign in setup for this. Follow this steps: https://developers.google.com/identity/protocols/oauth2/javascript-implicit-flow
- Once you have your client id, just put it in the env variable named 'REACT_APP_GOOGLE_CLIENT_ID' and **enable** the functionality with the env: 'REACT_APP_GOOGLE_SSO_ENABLED'.

# Cloning and runing this repo

1. Clone the repo with the subs: ``git clone --recurse-submodules -j8 https://github.com/DarwisNarvaezDev/fatsecret-nutrition-app.git``
2. go to /fatsecret-nutrition-app and create a simple '.env' file, you can work on top of the expample file in the repo, and expand all the variables in there.
3. Make sure that you have docker and docker-compose on your pc and run ``docker-compose up -d`` 
