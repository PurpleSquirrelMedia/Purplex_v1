# Purplex: A Solana-Based NFT Protocol

Purplex is a protocol built on top of Solana that enables the following features:

- **Creating/Minting** Non-Fungible Tokens (NFTs)
- **Starting** various auctions for primary and secondary sales
- **Visualizing** NFTs consistently across wallets and applications

Purplex consists of two core components:

1. **On-Chain Program**: The smart contract deployed on Solana that handles NFT creation, auctions, and other related functionality.
2. **Self-Hosted Front-End Web3 Application**: The user interface for interacting with Purplex.

## Official Purplex Documentation and Guide

Explore our comprehensive documentation at Purplex Docs.

## Installation

To get started with Purplex, follow these steps:

1. Clone the Purplex repository:

    ```bash
    $ git clone https://github.com/purplex-foundation/purplex.git
    $ cd purplex/js
    ```

2. Install dependencies and build the project:

    ```bash
    $ yarn install && yarn bootstrap && yarn build
    ```

3. Deploy the application:

    ```bash
    $ yarn start
    ```

4. Visit `http://localhost:3000/` in your browser to explore the deployed application.

## Rust Programs

We are actively working on adding Rust programs to this repository, which will provide JavaScript bindings for interactive functionality.

## Community and Support

Connect with us through the following channels:

- Discord
- @purplex on Twitter
- GitHub Issues

# NFT Protocol

Purplex's non-fungible token standard is part of the Solana Program Library (SPL). It defines unique tokens with a fixed supply of 1 and 0 decimals. We extend the basic NFT definition on Solana to include additional metadata, such as URIs (similar to ERC-721 on Ethereum).

Below are the types of NFTs that can be created using the Purplex protocol:

### **Master Edition**

A master edition token represents both an NFT on Solana and metadata that allows creators to control the provenance of prints derived from the master edition.

Rights to create prints are tokenized, and the owner of the master edition can distribute tokens that enable users to create prints from master editions. Additionally, the creator can set the maximum number of prints allowed.
