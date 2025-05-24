- fork repository 
- clone locally 
- setup remote upstream `git remote add upstream git@github.com:patrickalphac/foundry-fund-me-cu.git`

## Foundry Commands 
`````
$ forge install foundry-rs/forge-std
<!-- incase of an error remove the file or folders then run the command again -->
$ rm -rf lib/forge-std
$ forge install foundry-rs/forge-std
$ forge clean
$ forge build
$ forge script script/DeployFundMe.s.sol
$ forge test
$ forge test -vv
$ forge script DeployFundMe
$ forge coverage
$ forge test --mt testFundUpdatesFundedDataStructure
$ forge test --mt testAddsFunderToArrayOfFunders
$ forge test --mt testOnlyOwnerCanWithdraw
$ forge test --mt testWithdrawFromASingleFunder
$ forge test
$ forge test --mt testWithdrawFromMultipleFunders
$ forge test
$ forge coverage
$ forge snapshot --mt testWithdrawFromASingleFunder
$ forge test --mt testWithdrawFromASingleFunder -vv
`````



``````
$ forge install Cyfrin/foundry-devops --no-commit
$ forge script script/Interactions.s.sol:FundFundMe --rpc-url xyz --private-key etc ...
$ forge test --mt testUserCanFundAndOwnerWithdraw -vv
``````

## Summary of this Project 
### Recap

Let's quickly go through what we learned in this one:

* We learned more about how to set up a Foundry project

* We learned how to organize our files into folders, following the convention

* We learned how to refactor smart contracts to make them modular and chain-agnostic

* We learned how to write scripts that act as interaction commands

* We learned more about using mocks

* We did a bunch of unit tests, we even did an integration test

* We learned a bit about Makefiles

* We learned how to create a GitHub repository and push our code in it

* We also learned how to clone a GitHub repository

## Acknowledgement 
- [Cyfrin Updaft](https://updraft.cyfrin.io/courses/foundry/foundry-fund-me) Team and [Patrick Collins](https://x.com/PatrickAlphaC)
