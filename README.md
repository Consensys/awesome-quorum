# Awesome Quorum

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome softwares, libraries, tools, articles, educational resources, discussion channels and more to build on [ConsenSys Quorum](https://consensys.net/quorum/)

ConsenSys Quorum is a foundational open-source protocol layer that enables Enterprise Ethereum blockchain. It provides an extensive set of software components such as Enterprise Ethereum clients, private transactions managers, private key managers, plugins, libraries... to build decentralized platforms. ConsenSys Quorum is maintained by both engineering teams at [ConsenSys](https://consensys.net/) and the open-source community :heart:

Contributions to this list are wery welcome :dolphin: You can add links through [pull requests](https://github.com/ConsenSys/awesome-quorum/pulls) or create an [issue](https://github.com/ConsenSys/awesome-quorum/issues). Please take a look at the [contribution guidelines](CONTRIBUTING.md).

## Contents

- [Sofware components](#sofware-components)
  - [Enterprise Ethereum Clients](#enterprise-ethereum-client)
  - [Private Transaction Managers](#private-transaction-manager)
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
- [Community](#community)
  - [Wikis](#wikis)
  - [Chats](#chats)
  - [Meetups](#meetups)
  - [Events Calendar](#events-calendar)
  - [Developer Forums](#developer-forums)
- [Educational Resources](#educational-resources)
  - [Articles](#articles)
  - [Webinars](#webinars)
  - [Videos](#videos)
- [Contribute](#contribute)
  - [Contribution guidelines](#contribution-guidelines)
  - [Ambassador Program](#ambassador-program)
- [Built on Quorum](#built-on-quorum)
  - [Ecosystem directory](#ecosystem-directory)
  - [Enterprise use cases](#enterprise-use-cases)
  - [Third party tools, platform, projects](#third-party-tools-platform-projects)

## Sofware components

### Enterprise Ethereum Client

- [GoQuorum](https://github.com/ConsenSys/quorum) - Enterprise Ethereum client, fork of Go-Ethereum (aka Geth), compatible with permissioned networks and widely used in production
- [Hyperledger Besu](https://github.com/hyperledger/besu) - Enterprise Ethereum client written in Java under Apache 2.0 license, compatible with both public and permissioned networks

### Private Transaction Manager

- [Tessera](https://github.com/ConsenSys/tessera) - Stateless Java system enabling encryption, decryption, and distribution of private transactions for Quorum
- [Orion](https://github.com/ConsenSys/orion) - Private transaction manager developed under the Apache 2.0 license and written in Java

### Private Key Manager

- [EthSigner](https://github.com/ConsenSys/ethsigner) - Transaction signing application to be used with a web3 provider

### Plugins

- [Quorum Plugin Definitions](https://github.com/ConsenSys/quorum-plugin-definitions) - Extends Quorum functionality with gRPC based plugin API. Contains protobuf files defining plugin interfaces (e.g. Account plugin, Security plugin...)
- [Quorum Hashicorp Account Plugin](https://github.com/ConsenSys/quorum-account-plugin-hashicorp-vault) - Plugin enabling storage of Quorum account private keys in a Hashicorp Vault KV v2 secret engine.
- [Quorum Security Plugin](https://github.com/ConsenSys/quorum-security-plugin-enterprise) - Plugin enabling securing JSON-RPC server endpoints by adding TLS and support for OAuth2 based authentication
- [Besu Plugins](https://github.com/ConsenSys/besu-plugins/) - Extends Hyperledger Besu functionality using Java based plugin API to retrieve data from any Besu network, public or permissioned and feed it into an application or system
- [Besu Event Stream](https://github.com/ConsenSys/besu-plugins/tree/master/event-stream) - Besu plugin listening to events occurring on Ethereum network and broadcasting them to Kafka

### Libraries

- [quorumjs](https://github.com/ConsenSys/quorum.js) - Extension for web3.js which adds support for APIs specific to Quorum
- [web3js-eea](https://github.com/ConsenSys/web3js-eea) - Extension for web3.js which adds support for Besu private transaction and privacy group management
- [web3j-quorum](https://github.com/web3j/web3j-quorum) - An extension to web3j providing support for Quorum APIs

### Tools

- [Cakeshop](https://github.com/ConsenSys/cakeshop) - Set of tools and APIs for working with Ethereum-like ledgers, packaged as a Java web application archive
- [Quorum Remix](https://github.com/ConsenSys/quorum-remix) - Quorum plugin for Ethereum's Remix IDE adds support for creating and interacting with private contracts on a Quorum network
- [Quorum reporting](https://github.com/ConsenSys/quorum-reporting) - Tool that indexes blocks and transactions in a Quorum network and generates reports to give users insights into what is happening with their contracts
- [Besu permissioning dApp](https://github.com/ConsenSys/permissioning-smart-contracts) - Facilitate managing permissioning rules and maintaining the list of admin accounts that can edit rules
- [Istanbul Tools](https://github.com/ConsenSys/istanbul-tools) - Tools for configuring Istanbul BFT (IBFT) network

### Testing

- [GoQuorum Acceptance Test](https://github.com/ConsenSys/quorum-acceptance-tests) - Acceptance Tests for GoQuorum

### Performances

- [Quorum Profiling](https://github.com/ConsenSys/quorum-profiling) - Toolset built for the purpose of running stress tests on networks running on Quorum and measure/monitor the TPS and other benchmarking parameters at network level

## Deployment

### Sandbox

- [Quorum-Wizard](https://github.com/ConsenSys/quorum-wizard) - A command line tool that allow users to set up a development Quorum network on their local machine in less than 2 minutes
- [Quorum-Dev-Quickstart](https://github.com/ConsenSys/quorum-dev-quickstart) - A command line tool that allow users to set up a development Quorum network on their local machine in less than 2 minutes
- [Quorum Examples](https://github.com/ConsenSys/quorum-examples) - Setup examples to start a fully-functioning Quorum environment consisting of 7 independent nodes allowing to test consensus, privacy, and all the expected functionality of an Quorum platform

### Kubernetes

- [qubernetes](https://github.com/ConsenSys/qubernetes) - Generates the necessary Quorum resources (keys, configs - genesis, istanbul, etc.) and Kubernetes API resource yaml for a configurable Quorum Network
- [Quorum Kubernetes](https://github.com/ConsenSys/quorum-kubernetes) - Example reference implementations of private networks using k8s, intended for developers and ops to get familiar with private ethereum network in k8s

### Cloud

- [Quorum AWS](https://github.com/ConsenSys/quorum-aws) - Tools to deploy Quorum networks to AWS using Docker and Terraform

## Documentations

### Products

- [GoQuorum doc](https://docs.goquorum.consensys.net)
- [Orion doc](https://docs.orion.consensys.net)
- [Tessera doc](https://docs.tessera.consensys.net)
- [EthSigner doc](https://docs.ethsigner.consensys.net)
- [Orchestrate doc](https://docs.orchestrate.consensys.net)

### Specifications

- [EEA Technical specifications](https://entethalliance.org/technical-specifications/) - EEA’s world-class specifications and forth-coming testing and certification programs helps ensurnig interoperability between software components from multiple vendors
- [BFT specifications](https://github.com/ConsenSys/quorum-ibft) - Paper describing the BFT Consensus Algorithm, a simple and elegant algorithm for Byzantine fault-tolerant consensus and is used to implement state machine replication in the Quorum blockchain
- [RAFT specifications](https://raft.github.io/raft.pdf) - Paper describing the RAFT algorithm used by GoQuorum

## Community

### Website

- [ConsenSys Quorum](https://consensys.net/quorum)

### Wikis

- [Hyperledger wiki](https://wiki.hyperledger.org/) - Hyperledger is an open source collaborative effort created to advance cross-industry blockchain technologies. It is a global collaboration, hosted by The Linux Foundation, including leaders in finance, banking, IoT, supply chain, manufacturing and technology

### Chats

- [Quorum discord](https://discord.gg/kEJYV8XQuH)
- [GoQuorum Slack](https://inviter.quorum.consensys.net/)

### Meetups

### Events Calendar

### Developer Forums

## Educational Resources

### Articles

- [January 2021 - ConsenSys Quorum available on China blockchain services](https://consensys.net/blog/press-release/consensys-announces-partnership-with-chinas-blockchain-services-network/)
- [December 2020 - A Year in Review: ConsenSys Quorum Highlights](https://consensys.net/blog/quorum/a-year-in-review-consensys-quorum-highlights/)
- [November 2020 - ConsenSys Quorum Product Update: Bundles, Support and Leading Features](https://consensys.net/blog/news/consensys-quorum-november-2020-product-update-bundles-support-and-leading-features/)
- [October 2020 - ConsenSys Quorum is moving to Calendar Versioning](https://consensys.net/blog/news/consensys-quorum-is-moving-to-calendar-versioning/)
- [August 2020 - ConsenSys acquires JPM Quorum](https://consensys.net/blog/news/consensys-acquires-jpm-quorum/)
- [January 2020 - EEA Testnet launch](https://consensys.net/blog/enterprise-blockchain/what-the-eea-testnet-launch-means-for-blockchain-and-enterprise/)

### Webinars

- [Web3j and ConsenSys Quorum](https://pages.consensys.net/web3j-and-consensys-quorum)
- [Getting Started With ConsenSys Quorum](https://pages.consensys.net/getting-started-with-consensys-quorum)
- [Introducting ConsenSys Quorum](https://pages.consensys.net/introducing-consensys-quorum)

### Videos

## Contribute

### Contribution guidelines

### Ambassador Program

## Built on Quorum

### Ecosystem directory

### Enterprise use cases

### Third party tools, platform, projects
