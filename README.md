![](https://i.imgur.com/4GO7nnY.png)

Wallet Wasabi, formerly known as HiddenWallet is a [ZeroLink](https://github.com/nopara73/ZeroLink) compliant Bitcoin wallet. We are dedicated to restore Bitcoin's fungibility and provide the highest possible privacy for our users.  
HiddenWallet's code is archived in the [hiddenwallet-v0.6](https://github.com/zkSNACKs/WalletWasabi/tree/hiddenwallet-v0.6) branch of this repository.

| Windows | Linux & OSX
| :---- | :------ |
[![Windows build status][1]][2] | [![Linux & OSX build status][3]][4] |

[1]: https://ci.appveyor.com/api/projects/status/70j293muovayg516?svg=true
[2]: https://ci.appveyor.com/project/zkSNACKs/walletwasabi
[3]: https://travis-ci.org/zkSNACKs/WalletWasabi.svg?branch=master
[4]: https://travis-ci.org/zkSNACKs/WalletWasabi

## Roadmap

**Goal:** Stability, feature minimalization.

It is expected for the proposed timeline to take roughly 1.5 times longer.

### 1. Wallet Stage

- [x] **1. Wallet Back End.** *2 weeks. NBitcoin, Bitcoin Core RPC, ASP.NET.* Build back end.
- [x] **2. Small Tor Library.** *1 week. Tor, .NET Core, cross platform.* Build a small Tor library based on DotNetTor, that removes features those are unrelated to the wallet and makes the rest more stable.
- [x] **3. Key Manager.** *1 week. NBitcoin.* Build a new, high performance key manager with accounts, labelling, etc...
- [x] **4. Wallet Client.** *1 month. NBitcoin.* Build a high performance client that can work with the new back end, which is built for client side filtering.

  Depends on:
  - [x] ALL previous items
  
### 2. Privacy Stage

- [x] **5. ZeroLink Research.** *1 month. Bitcoin privacy, cryptography.* Research ZeroLink, based on technological advancements.
- [x] **6. ZeroLink Coordinator.** *2 weeks. NBitcoin, Bitcoin Core RPC.* Revise the ZeroLink Coordinator code based on ZeroLink v2 Revision.

  Depends on:
  - [x] ZeroLink Research
  
- [ ] **7. ZeroLink Client.** *2 weeks. NBitcoin.* Revise the ZeroLink Client code based on ZeroLink v2 Revision.

  Depends on:
  - [x] ZeroLink Research
  - [ ] ZeroLink Coordinator

### 3. User Experience Stage

- [ ] **8. GUI.** *1 month. Electron, front end, Bitcoin.* Redesign the user experience and build it.

  Depends on:
  - [ ] ALL previous items
  
### 4. Deployment Stage
  
- [ ] **9. Documentation.** *1 week. Bitcoin.* Create documentation.

  Depends on:
  - [ ] ALL previous items
  
- [ ] **10. Internal Testing.** *2 weeks. Bitcoin or .NET or front end.* Test the software and fix the bugs (if there is any haha).

  Depends on:
  - [ ] ALL previous items, except Documentation
  
- [ ] **11. Deploy To Mainnet.** *2 weeks. .NET Core, ASP.NET Core deployment.* Deploy the software to Bitcoin Mainnet.

  Depends on:
  - [ ] ALL previous items, except Documentation
  
- [ ] **12. Mainnet Beta Testing.** *2 weeks.* It's rather a marketing phase. The goal is to get at least 1 round done with > 100 user.

  Depends on:
  - [ ] ALL previous items
  
