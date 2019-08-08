# Hydra X Trader

## Directory structure

src/*.tsx: React UI components

src/modules.ts: Module loader

src/hydra_api.ts: Hydra API functions for modules

src/models/*.ts: Data models 

## Installing dependencies

```
npm install
```

## Running Webtrader

```
Development: npm run start-dev
Production: npm run start-prod
```

## Deploying Webtrader

```
Webtrader : npm run deploy-web
Webtrader Test: npm run deploy-web-test
Webtrader Test 2: npm run deploy-web-test-2

```

Access `http://localhost:8080/` in browser


## Forcing users to reload local config file

Within app.tsx, there is a new feature to enable us to force users to reset their workspace layout and settings data.
‘cacheversion’ retrieves a string from the user’s cache and compares it to the string ‘configversion’ in our app to produce a variable ‘versionmatch’ which will be used as part of the checks to determine if the user’s configuration should be reloaded.

Changing the ‘configversion’ variable in line 97 of app.tsx will force users to reload their configuration files.
```
var configversion = "0.1.0";
```
Note: Neither ‘cacheversion’ nor ‘configversion’ pertains to the app version displayed to the users. The app version displayed can be changed separately.
