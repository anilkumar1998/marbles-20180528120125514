# Marbles Demo Notes

[![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/ibm-blockchain/marbles.git)

## Doc Links
- obc.js SDK Doc - [utils/obc-js](./utils/obc-js/README.md)
- Tutorial for Marbles Phase 1 - [here](./phase1_tutorial.md) (start here)
- Tutorial for Marbles Phase 2 - coming

***

## Projects Contents
1. **JS sdk** - `./utils/obc-js`
1. **Marbles Demo**   -	http://localhost:3000

***

## Demo Phase 1 Goals
- [x] User can create a marble and store it in the chaincode state
- [x] User can read all marbles in the chaincode state
- [x] User can transfer marble to another user
- [x] See block stats
- [x] User can delete a marble
- [x] Deployable on bluemix

## Demo Phase 2 Goals
- [x] Server pushes block/marble updates to client when a new block event has occured for local user
- [x] User's can advertise to trade/exchange their marbles (ie willing to trade large red for large blue/yellow/green)
- [ ] User can remove their open trades
- [x] User identity (fake login as bob or leroy)
- [x] Ability to see past blocks details and some sort of animation on new blocks

## Demo Phase 3 Goals
- [ ] Server pushes block/marble updates to client when any new block event has occured
- [ ] User autentication (crypto signing of transactions)
- [ ] User registration
- [ ] Transacation privacy

***

## ChainCode / SDK ToDo:
- [x] Write("name", "val", cb);
- [x] ReadNames(cb)
- [x] init_marble(json);
- [ ] check permissions of requesting user in cc
- [ ] verify user identity, ie public private key stuff
- [x] website to test cc, real basic
- [x] demo app website
- [x] make sdk proper npm module
- [x] custom custom function on UI
- [x] load json in UI
- [x] structured error reponse
- [ ] mocha test for sdk
- [ ] browsify sdk and tie cci into it (not sure if i want to)
- [ ] change downloading zip to git clone
- [x] follow redirect on zip download
- [x] auto deploy, correctly!
- [x] get delete to update marbleIndex
- [x] sdk, check inputs on load if they  dne, error
- [o] poll after chain deploy for cc up in peer [can't, future auth will prevent]
- [x] add block stats to sdk
- [x] write tutorial on phase 1
- [ ] move to socket.io (unsure, postpone)
- [x] change test var "a" to "abc" in cc
- [x] make advanced link in cci and hide ip/port fields, hide all things under tool like categories
- [x] make CCI work for multiple apps, pick which cc to load (even custom functions)
- [x] block history UI
- [ ] CCI video
- [ ] CCI screens with filled out info
- [x] restyle marbles to match new design
- [ ] multi marble on willing list
- [ ] remove/edit trades that are no longer possible in CC
- [ ] remove named marble argument on perform_trade message/golang func, replace with color/size thing
- [ ] check requirments of trade before exe, in CC
- [ ] error checking on arguements before invoking... do not let e blank named marble in
- [x] url routing mapper
- [ ] improve marble redraw so we don't have to blank the marble divs
- [ ] tutorial for p2
- [ ] re-parallelize the queryies
- [x] show open trades made by user
- [ ] ability to remove open trades by user
- [ ] make layout adaptive
- [ ] sanitize git url to make sure it looks right... should not have .git
