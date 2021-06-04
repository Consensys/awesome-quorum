# Awesome Quorum

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome softwares, libraries, tools, articles, educational resources, discussion channels and more to build on [ConsenSys Quorum](https://consensys.net/quorum/)

ConsenSys Quorum is a foundational open-source protocol layer that enables Enterprise Ethereum blockchain. It provides an extensive set of software components such as Enterprise Ethereum clients, private transactions managers, private key managers, plugins, libraries... to build decentralized platforms. ConsenSys Quorum is maintained by both engineering teams at [ConsenSys](https://consensys.net/) and the open-source community :heart:

Contributions to this list are wery welcome :dolphin: You can add links through [pull requests](https://github.com/ConsenSys/awesome-quorum/pulls) or create an [issue](https://github.com/ConsenSys/awesome-quorum/issues).

## Contents

- [Software components](#software-components)
  - [Enterprise Ethereum Clients](#enterprise-ethereum-client)
  - [Private Transaction Manager](#private-transaction-manager)
  - [Private Key Mangager](#private-key-manager)
  - [Plugins](#plugins)
  - [Libraries](#libraries)
  - [Tools](#tools)
  - [Testing](#testing)
  - [Performances](#performances)
- [Deployment](#deployment)
  - [Sandbox](#sandbox)
  - [Kubernetes](#kubernetes)
  - [Cloud](#cloud)
- [Documentations](#documentations)
  - [Products](#products)
  - [Specifications](#specifications)
- [Contribute](#contribute)  
- [Community](#community)
  - [Wikis](#wikis)
  - [Chats](#chats)
  - [Events](#events)
  - [Developer Forums](#developer-forums)
  - [Ambassador Program](#ambassador-program)
- [Educational Resources](#educational-resources)
  - [Articles](#articles)
  - [Webinars](#webinars)
  - [Videos](#videos)
- [Built on Quorum](#built-on-quorum)

## Software components

### Enterprise Ethereum Client

- [Hyperledger Besu](https://github.com/hyperledger/besu) - Enterprise Ethereum client written in Java under Apache 2.0 license, compatible with both public and permissioned networks
- [GoQuorum](https://github.com/ConsenSys/quorum) - Enterprise Ethereum client, fork of Go-Ethereum (aka Geth), compatible with permissioned networks and widely used in production

### Private Transaction Manager

- [Tessera](https://github.com/ConsenSys/tessera) - Stateless Java system enabling encryption, decryption, and distribution of private transactions for Quorum
- [Orion](https://github.com/ConsenSys/orion) - Private transaction manager developed under the Apache 2.0 license and written in Java

### Private Key Manager

- [EthSigner](https://github.com/ConsenSys/ethsigner) - Transaction signing application to be used with a web3 provider
- [Quorum Signer Hashicorp](https://github.com/ConsenSys/quorum-signer-plugin-for-hashicorp-vault) -  Custom plugin backend for Hashicorp Vault adding a new `quorum-signer` secret-engine to Hashicorp Vault

### Plugins

- [Quorum Plugin Definitions](https://github.com/ConsenSys/quorum-plugin-definitions) - Extends Quorum functionality with gRPC based plugin API. Contains protobuf files defining plugin interfaces (e.g. Account plugin, Security plugin...)
- [Quorum Hashicorp Account Plugin](https://github.com/ConsenSys/quorum-account-plugin-hashicorp-vault) - Plugin enabling storage of Quorum account private keys in a Hashicorp Vault KV v2 secret engine.
- [Quorum Security Plugin](https://github.com/ConsenSys/quorum-security-plugin-enterprise) - Plugin enabling securing JSON-RPC server endpoints by adding TLS and support for OAuth2 based authentication
- [Quorum Remix IDE Plugin](https://github.com/ConsenSys/quorum-remix) - The Quorum plugin for Ethereum's Remix IDE adds support for creating and interacting with private contracts on a Quorum network.
- [Besu Plugins](https://github.com/ConsenSys/besu-plugins/) - Extends Hyperledger Besu functionality using Java based plugin API to retrieve data from any Besu network, public or permissioned and feed it into an application or system
- [Besu Event Stream](https://github.com/ConsenSys/besu-plugins/tree/master/event-stream) - Besu plugin listening to events occurring on Ethereum network and broadcasting them to Kafka

### Libraries

- [quorumjs](https://github.com/ConsenSys/quorum.js) - Extension for web3.js which adds support for APIs specific to Quorum
- [web3js-eea](https://github.com/ConsenSys/web3js-eea) - Extension for web3.js which adds support for Besu private transaction and privacy group management
- [web3j-quorum](https://github.com/web3j/web3j-quorum) - An extension to web3j providing support for Quorum APIs
- [Truffle with Quorum](https://www.trufflesuite.com/docs/truffle/distributed-ledger-support/working-with-quorum) - Truffle supports development with Quorum, a version of Ethereum that adds new features on top of what Ethereum already provides
- [Nethereum](https://docs.nethereum.com/en/latest/ethereum-and-clients/quorum/) - Nethereum is the .Net integration library for Ethereum, simplifying smart contract management and interaction with Ethereum nodes whether they are public, like Geth , Parity or private, like Quorum and Besu.
- [Quorum-toolbox](https://github.com/chainstack/quorum-toolbox) - Tools and scripts for Quorum configuration.
- [Web3Quorum](https://github.com/chainstack/web3quorum) - A web3py extension that supports Quorum APIs: Raft and Istanbul.

### Interoperability 
- [Cordage](https://github.com/LayerXcom/cordage) - Cordage makes the interoperability possible from Corda to Quorum and Hyperledger Besu by providing several modules that propagate, pull and verify information between Blockchains without further trusted third party.
- [Wanchain](https://github.com/wanchain/T-Bridge-Contracts) - Wanchain Trust Bridge currently provides a reference implementation to connect Wanchain to a private blockchain built with Hyperledger Besu originally from Consensys. 

### Tools

- [Cakeshop](https://github.com/ConsenSys/cakeshop) - Set of tools and APIs for working with Ethereum-like ledgers, packaged as a Java web application archive
- [Quorum Remix](https://github.com/ConsenSys/quorum-remix) - Quorum plugin for Ethereum's Remix IDE adds support for creating and interacting with private contracts on a Quorum network
- [Quorum reporting](https://github.com/ConsenSys/quorum-reporting) - Tool that indexes blocks and transactions in a Quorum network and generates reports to give users insights into what is happening with their contracts
- [Besu permissioning dApp](https://github.com/ConsenSys/permissioning-smart-contracts) - Facilitate managing permissioning rules and maintaining the list of admin accounts that can edit rules
- [Istanbul Tools](https://github.com/ConsenSys/istanbul-tools) - Tools for configuring Istanbul BFT (IBFT) network
- [Quorum-Splunk](https://www.splunk.com/en_us/blog/it/introducing-splunk-app-for-quorum.html) - Using Splunk for quorum blockchain analytics and dashboards
- [Mirror Besu](https://www.npmjs.com/package/mirror-besu) - compiling, testing and deployment for Hyperledger Besu, aiming to make life as an Enterprise Ethereum developer easier.
- [Ethernal](https://tryethernal.com/) - Block explorer for private EVM-based chains.

### Testing

- [GoQuorum Acceptance Test](https://github.com/ConsenSys/quorum-acceptance-tests) - Acceptance Tests for GoQuorum

### Performances

- [Quorum Profiling](https://github.com/ConsenSys/quorum-profiling) - Toolset built for the purpose of running stress tests on networks running on Quorum and measure/monitor the TPS and other benchmarking parameters at network level
- [gohammer](https://github.com/tubuarge/gohammer) - Quorum and Besu TPS performance tool written in golang. Based on scenario configuration to load transactions to your network. 

## Deployment

### Sandbox

- [Quorum-Dev-Quickstart](https://github.com/ConsenSys/quorum-dev-quickstart) - Deploy up a ConsenSys Quorum network on your local machine from the command line in only a few minutes
- [Quorum-Wizard](https://github.com/ConsenSys/quorum-wizard) - A command line tool that allow users to set up a development Quorum network on their local machine in less than 2 minutes
- [Quorum Examples](https://github.com/ConsenSys/quorum-examples) - Setup examples to start a fully-functioning Quorum environment consisting of 7 independent nodes allowing to test consensus, privacy, and all the expected functionality of an Quorum platform
- [Quorum Network Manager (deprecated)](https://github.com/ConsenSys/QuorumNetworkManager) - basic way for originally getting started with a quorum network
- [Quorum Maker](https://github.com/synechron-finlabs/quorum-maker) - Synechron's Quorum Maker is a tool that allows users to create and manage Quorum network
- [Besu Truffle Box](https://www.trufflesuite.com/boxes/besu-box) - Truffle Box Creating API Endpoints for Hyperledger Besu network.
- [Epirus Free - Blockchain Explorer](https://github.com/web3labs/epirus-free) - This dockerized environment is designed for viewing private Quorum, Pantheon and Ethereum networks.
- [Greenhouse by BlockTEST](https://greenhouse.blocktest.com/home) - an integrated toolbox for blockchain DevOps, an automated middleware development platform as a service, so that you can build blockchain applications in a streamlined way and on consistent sets of architectural plumbing principles
- [Platform6](https://platform6.io/) - provides all the off-chain features and services required to develop, package and run enterprise-class decentralized applications for Besu and GoQuorum.
- [Tubu.io](https://www.tubu.io/) - create and manage ConsenSys Quorum/ private blockchain applications  

### Kubernetes

- [qubernetes](https://github.com/ConsenSys/qubernetes) - Generates the necessary Quorum resources (keys, configs - genesis, istanbul, etc.) and Kubernetes API resource yaml for a configurable Quorum Network
- [Quorum Kubernetes](https://github.com/ConsenSys/quorum-kubernetes) - Example reference implementations of private networks using k8s, intended for developers and ops to get familiar with private ethereum network in k8s

### Cloud

- [Quorum Terraform Provider](https://registry.terraform.io/providers/ConsenSys/quorum/latest) - The Quorum provider is used to bootstrap various resources required to create a running Quorum Network
- [Quorum AWS](https://github.com/ConsenSys/quorum-aws) - Tools to deploy Quorum networks to AWS using Docker and Terraform
- [Azure Blockchain Service](https://docs.microsoft.com/en-us/azure/blockchain/service/develop) - create consortium blockchain networks to enable enterprise scenarios like asset tracking, digital token, loyalty and reward, supply chain financial, and provenance.
- [SAP Cloud Platform](https://blogs.sap.com/2019/01/11/quorum-on-sap-cloud-platform/) - now offers a free-of-charge “dev” service plan for developers to build with Quorum in a playground environment. The plan offers Quorum instances that are shared with other developers.
- [Chainstack](https://chainstack.com/) - Managed blockchain services making it simple to launch and scale decentralized networks and applications for ConsenSys Quorum
- [Blockdaemon](https://app.blockdaemon.com/marketplace) - Infrastructure and testing provider where you can deploy ConsenSys Quorum in a few steps, decentralize your infrastructure with multiple cloud providers, white-label your own control panel and integrate existing systems or APIs.

## Documentation

### Products

- [Besu docs](https://besu.hyperledger.org/en/stable/)
- [GoQuorum docs](https://docs.goquorum.consensys.net)
- [Orion docs](https://docs.orion.consensys.net)
- [Tessera docs](https://docs.tessera.consensys.net)
- [EthSigner docs](https://docs.ethsigner.consensys.net)
- [Orchestrate docs](https://docs.orchestrate.consensys.net)

### Specifications

- [GoQuorum whitepaper](https://github.com/ConsenSys/quorum/blob/master/docs/Quorum%20Whitepaper%20v0.2.pdf)
- [EEA Technical specifications](https://entethalliance.org/technical-specifications/) - EEA’s world-class specifications and forth-coming testing and certification programs helps ensuring interoperability between software components from multiple vendors
- [BFT specifications](https://github.com/ConsenSys/quorum-ibft) - Paper describing the BFT Consensus Algorithm, a simple and elegant algorithm for Byzantine fault-tolerant consensus and is used to implement state machine replication in the Quorum blockchain
- [RAFT specifications](https://raft.github.io/raft.pdf) - Paper describing the [RAFT algorithm](https://raft.github.io/) used by GoQuorum

## Contribute

- [Contribute to GoQuorum](https://github.com/ConsenSys/quorum/blob/master/.github/CONTRIBUTING.md)
- [Contribute to Besu](https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md)

## Community

### Website

- [ConsenSys Quorum](https://consensys.net/quorum)

### Wikis

- [Hyperledger wiki](https://wiki.hyperledger.org/) - Hyperledger is an open source collaborative effort created to advance cross-industry blockchain technologies. It is a global collaboration, hosted by The Linux Foundation, including leaders in finance, banking, IoT, supply chain, manufacturing and technology
- [GoQuorum Wiki](https://github.com/ConsenSys/quorum/wiki)

### Chats

- [Discord](https://bit.ly/ConsenSysQuorumDiscord)
  - [Slack - GoQuorum](https://inviter.quorum.consensys.net/)
  - [Rocketchat - Hyperledger Besu](http://chat.hyperledger.org/)

### Events
- [ConsenSys Quorum Event Calendar]
- [Hyperledger Besu Event Calendar]

### Developer Forums

- [Stack Overflow Quorum](https://stackoverflow.com/questions/tagged/quorum)
- [Stack Overflow Besu](https://stackoverflow.com/search?q=hyperledger+besu)
- [Stack Exchange Quorum](https://ethereum.stackexchange.com/questions/tagged/quorum)
- [Stack Exchange Besu](https://ethereum.stackexchange.com/questions/tagged/besu)

### Ambassador Program
- [Apply to be a ConsenSys Quorum Ambassador!](https://bit.ly/ConsenSysAmbassadorApp)

## Educational Resources
- [Quorum Workshop - MLH](https://github.com/dyelax/quorum-workshop)
- [Quorum Workshop - Blockmatics](https://blockmatics.teachable.com/p/quorum-blockchain-developer-course)
- [Blockgeeks Guide: Overview of GoQuorum](https://blockgeeks.com/guides/quorum-a-blockchain-platform-for-the-enterprise/)
- [B9Lab - Quorum Specialization Course](https://academy.b9lab.com/courses/course-v1:B9lab+QSE-X+2018-04/about)
- [Picking an enterprise blockchain protocol to develop on: Quorum, Vyper & Solidity](https://chainstack.com/picking-an-enterprise-protocol-to-develop-on-quorum/)
- [Food supply temperature control with Web3 on Quorum](https://docs.chainstack.com/tutorials/quorum/food-supply-temperature-control-with-web3)

### Articles

- [50+ Projects Building on J.P. Morgan's Quorum Blockchain](https://medium.com/@mateo_ventures/heres-who-s-building-on-quorum-see-the-list-b18d65aa0a2c)
- [ConsenSys Quorum available on China blockchain services](https://consensys.net/blog/press-release/consensys-announces-partnership-with-chinas-blockchain-services-network/)
- [A Year in Review: ConsenSys Quorum Highlights](https://consensys.net/blog/quorum/a-year-in-review-consensys-quorum-highlights/)
- [ConsenSys Quorum Product Update: Bundles, Support and Leading Features](https://consensys.net/blog/news/consensys-quorum-november-2020-product-update-bundles-support-and-leading-features/)
- [ConsenSys Quorum is moving to Calendar Versioning](https://consensys.net/blog/news/consensys-quorum-is-moving-to-calendar-versioning/)
- [ConsenSys acquires JPM Quorum](https://consensys.net/blog/news/consensys-acquires-jpm-quorum/)
- [EEA Testnet launch](https://consensys.net/blog/enterprise-blockchain/what-the-eea-testnet-launch-means-for-blockchain-and-enterprise/)

### Videos

- [Introducting ConsenSys Quorum](https://youtu.be/ItKg3P2Kmhs)
- [Getting Started with ConsenSys Quorum](https://youtu.be/CY2XOcnkV9o)
- [Web3j and ConsenSys Quorum](https://youtu.be/EC7PQtLvc2I)
- [Connecting Hyperledger Besu to Enterprise](https://youtu.be/93Mbdh4BvdM)
- [Using Quorum Remix IDE Extension](https://youtu.be/lT5y4hQLwUQ)
- [Quorum Features on Chainstack Demo](https://youtu.be/QPtqk3yPQK8)
- [Splunking with Quorum](https://youtu.be/Fo2qaEn1_BQ)

### Built on Quorum

- [7nodes](https://github.com/ConsenSys/quorum-examples/tree/master/examples/7nodes) - Starts up a fully-functioning
  GoQuorum environment consisting of 7 independent nodes.
  Demonstrates consensus, privacy, and all the expected functionality of an Ethereum platform.
- [web3j token sample](https://github.com/blk-io/quorum-sample) - Demonstrates the creation and management of a private
  token on a GoQuorum network.
  Written in Java using web3j which is maintained by Web3 Labs.
- [Pons bridge](https://github.com/M-Bowe/pons) | [Pons-Frontend](https://github.com/M-Bowe/pons-frontend) - A sample
  Cross-Chain Trading Bridge written to run over 2 GoQuorum Chains to safely exchange ERC-20 and ERC-721 assets.
- [Marketplace](https://github.com/lyotam/techmarketplace) - An example application running on top of a GoQuorum network
  which allows users to bid for and offer virtual hackathon gear for sale in an interactive marketplace.
  Based on what was originally developed for the MLH Localhost GoQuorum workshop.
- [ZSL proof of concept](https://github.com/ConsenSys/quorum/wiki/ZSL) - ZSL for GoQuorum enables the issuance of
  digital assets using ZSL-enabled public smart contracts (z-contracts).
  A combination of Tessera private contracts with z-contracts allows obligations that arise from a private contract to
  be settled using shielded transfers of z-tokens, while maintaining full privacy and confidentiality.
- [Anonymous Zether](https://github.com/ConsenSys/anonymous-zether/) - A private payment system; an anonymous extension
  of Bünz, Agrawal, Zamani, and Boneh's [Zether protocol](https://crypto.stanford.edu/~buenz/papers/zether.pdf).
