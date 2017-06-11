# Why this is here

Write the code (deployable to the EVM) that will be used to pay your salary, publish it on Github (public or private) and send link to repo plus any information you consider important to jorge@aragon.one, with the subject Solidity opening application.

https://gist.github.com/izqui/3428122070f2f8971c52f39c4d762252  

# truffle-init-webpack
Example webpack project with Truffle. Includes contracts, migrations, tests, user interface and webpack build pipeline.

## Usage

To initialize a project with this exapmple, run `truffle init webpack` inside an empty directory.

## Building and the frontend

1. First run `truffle compile`, then run `truffle migrate` to deploy the contracts onto your network of choice (default "development").
1. Then run `npm run dev` to build the app and serve it on http://localhost:8080

## Possible upgrades

* Use the webpack hotloader to sense when contracts or javascript have been recompiled and rebuild the application. Contributions welcome!

## Common Errors

* **Error: Can't resolve '../build/contracts/MetaCoin.json'**

This means you haven't compiled or migrated your contracts yet. Run `truffle compile` and `truffle migrate` first.

Full error:

```
ERROR in ./app/main.js
Module not found: Error: Can't resolve '../build/contracts/MetaCoin.json' in '/Users/tim/Documents/workspace/Consensys/test3/app'
 @ ./app/main.js 11:16-59
```
