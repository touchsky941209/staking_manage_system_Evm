# Staking token Project

This project is Staking management system on EVM.
Token is ERC-20 standard.

Try running some of the following tasks:

### project install

```shell
npm install
```
### project compile

```shell
npx hardhat compile
```
The result will be
```shell
Generating typings for: 42 artifacts in dir: typechain-types for target: ethers-v6
Successfully generated 126 typings!
Compiled 40 Solidity files successfully (evm target: paris).
```
### project test

```shell
npx hardhat test
```

The result will be 

```shell
Lock
    Deployment
      ✔ Should set the right unlockTime (633ms)
      ✔ Should set the right owner
      ✔ Should receive and store the funds to lock
      ✔ Should fail if the unlockTime is not in the future
    Withdrawals
      Validations
        ✔ Should revert with the right error if called too soon
        ✔ Should revert with the right error if called from another account
        ✔ Shouldn't fail if the unlockTime has arrived and the owner calls it
      Events
        ✔ Should emit an event on withdrawals
      Transfers
        ✔ Should transfer the funds to the owner


  9 passing (693ms)
```
