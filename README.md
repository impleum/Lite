| Windows | Mac OS | Linux
| :---- | :------ | :---- |
| [![Build status](https://dev.azure.com/StratisProject/Breeze/_apis/build/status/Hosted%20Windows%20Container?branchName=master)](https://dev.azure.com/StratisProject/Breeze/_build/latest?definitionId=10) | [![Build status](https://dev.azure.com/StratisProject/Breeze/_apis/build/status/Hosted%20macOS?branchName=master)](https://dev.azure.com/StratisProject/Breeze/_build/latest?definitionId=12) | [![Build status](https://dev.azure.com/StratisProject/Breeze/_apis/build/status/Hosted%20Ubuntu%201604?branchName=master)](https://dev.azure.com/StratisProject/Breeze/_build/latest?definitionId=11)

# Lite

__Warning: We're still in beta, so use at your own risk.__
This is the repository of the Lite Wallet, the first full-block SPV bitcoin wallet using Angular and Electron at the front-end and C# with .NET Core in the back-end.

## Daemon Build

Lite daemon is the backend REST service, hosting a Bitcoin node upon which Lite UI depends:

```
# Clone and go in the directory
git clone https://github.com/impleum/Lite
cd Lite

# Initialize dependencies
git submodule update --init --recursive

# Go in the Lite deamon folder
cd ImpleumBitcoinFullNode/Impleum.BreezeD
dotnet build

# Run the Bitcoin and Impleum full-SPV daemons on testnet in separate terminals
dotnet run
dotnet run impleum
```

## UI Build

[Read more...](https://github.com/impleum/Lite/blob/master/Lite.UI/README.md)

## CI Build
-----------

Every time someone pushes to the master branch or create a pull request on it, a build is triggered and a new unstable app release is created.

If you want the :sparkles: latest :sparkles: (unstable :bomb:) version of the Lite app, you can get it here: 

https://github.com/impleum/Lite/releases/tag/Continuous-Delivery

