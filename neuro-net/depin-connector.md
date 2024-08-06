# DePIN Connector

The DePIN Connector is a module that connects with DePIN(Decentralized Physical Infrastructure Networks). It provides a set of unified interfaces that integrate with different DePIN providers, and essential for enabling decentralized, real-time interactions with external data sources.&#x20;

## Why We Need Decentralized Data Sources?

Centralized data sources typically have risks of single points of failure and being tampered with. Using incorrect data sources on AI agents can have severe consequences:

1. **Faulty Decision Making**: AI agents relying on false data can make incorrect decisions, leading to poor or fatal outcomes in applications such as healthcare, navigation, and environmental monitoring.
2. **Security Risks**: Compromised data can lead to security vulnerabilities, exposing systems to attacks and malicious activities.
3. **Loss of Trust**: Inaccurate data erodes trust in AI systems and the entities that deploy them, undermining the adoption of AI technologies.

Decentralized data sources, provided by DePIN, can resolve the problems. It ensures data integrity, privacy, and resilience against malicious attacks and data falsification.

## Architecture Design

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

The DePIN Connector offers seamless access to external data interfaces. It uses decentralized protocols to ensure data integrity and security. The architecture includes:

* **API Gateways**: Provides a set of unified API interfaces, connecting to various data and tools providers from DePIN.
* **Data Validation**: Ensures data accuracy and reliability by cross-verifying similar data sources from different data providers to identify and select the most precise information.
* **Secure Data Channels**: Utilizing blockchain and cryptographic methods to secure data transfers.

## Proposed Partners to be Integrated

### Computing\&Storages

* [Aethir](https://aethir.com): Provides the decentralized computing power for training or fine-tuning the LLMs used by AI agents.
* [io.net](https://io.net): Provides GPU access worldwide and flexible and scalable clusters with auto scaling.
* [Filecoin](https://filecoin.io/): Provides decentralized storages and indexers.
* [Arweave](https://www.arweave.org/): Provides a permanent and decentralized web inside an open ledger.

### Data Sources

* [Hivemapper](https://www.hivemapper.com/): Provides map image and features data in a decentralized manner.
* [The Graph](https://thegraph.com/): Allows AI agents to query open APIs called subgraphs, to retrieve data that is indexed on the network.
* [NFTGo](https://nftgo.io/developers): Provides NFT data, trading and pricing API.

### Tools\&Services

* [Helium](https://www.helium.com/): Provides the access to the world's largest LoRaWAN network and fastest growing cellular network.
* [Aphone](https://www.aphone.com/): Offers access to and usage of a decentralized cloud smartphone.

