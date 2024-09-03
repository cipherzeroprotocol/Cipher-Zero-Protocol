Smart Contracts Guide
This document provides a comprehensive overview of the smart contracts used in the BitTheta Secure project, including details on deployment and interaction.

Table of Contents
Overview
Smart Contract Directory Structure
Deployment Instructions
Interaction Instructions
Contract Details
Overview
The BitTheta Secure project incorporates a suite of smart contracts designed to support various functionalities such as identity management, token management, staking, governance, and more. This guide details the directory structure, deployment processes, and methods for interacting with these contracts.

Smart Contract Directory Structure
The smart contracts are organized into the following directories:

IdentityManagement/
IdentityManagement.sol: Contracts related to identity management.
TokenManagement/
THETAStaking.sol: Implements staking mechanisms for THETA tokens.
Alvara/
deploy/: Deployment scripts for Alvara contracts.
deploy.js: Script for deploying Alvara contracts.
Alva.sol: Main contract for Alvara.
AlvaraGovernance.sol: Governance contract for Alvara.
AlvaraLending.sol: Lending functionality for Alvara.
AlvaraRewards.sol: Manages rewards for Alvara.
AlvaraStaking.sol: Staking functionality for Alvara.
AlvaraVault.sol: Vault for storing assets.
BTS.sol: BTS token contract.
BTSFactory.sol: Factory for creating BTS tokens.
BTSMarketplace.sol: Marketplace for BTS tokens.
BTSPair.sol: Token pair contract for BTS.
ERC-BTS.sol: ERC-BTS token standard implementation.
Factory.sol: Factory for Alvara-related contracts.
HiveX.sol: Marketplace and ecosystem integration.
Banking Integration/
banking_contract.sol: Integrates banking functionalities.
BitTheta Secure/
Analytics/
Analytics.sol: Provides analytics functionality.
RealTimeMonitoring.sol: Real-time monitoring services.
UsageAnalytics.sol: Usage analytics.
Automation/
EscrowServices.sol: Escrow services.
OracleIntegration.sol: Integrates with oracles.
Community/
CommunityChannels.sol: Manages community channels.
SocialSharing.sol: Social sharing functionalities.
CrossChain/
CrossChainTransfers.sol: Handles cross-chain transfers.
Interoperability.sol: Ensures interoperability.
Encryption/
EndToEndEncryption.sol: Provides end-to-end encryption.
Verifier.sol: Verifies encrypted data.
Gamification/
AchievementsBadges.sol: Manages achievements and badges.
ChallengesContests.sol: Handles challenges and contests.
Identity/
DIDIntegration.sol: Integrates Decentralized Identifiers (DID).
ReputationSystem.sol: Manages reputation systems.
Incentives/
FileSharingIncentives.sol: Incentives for file sharing.
Staking.sol: Staking functionalities.
VideoStreaming/
LiveStreaming.sol: Live streaming functionalities.
OnDemandContent.sol: On-demand content services.
Bridges/
CrossChainToken.sol: Manages cross-chain tokens.
WormholeBridge.sol: Integrates Wormhole bridge.
Governance/
Governance.sol: Governance contract.
IGovernance.sol: Governance interface.
SubchainGovernanceToken.sol: Token for governance.
Sustainability/
eco_friendly_contract.sol: Contracts for eco-friendly initiatives.
Infrastructure/
base/
Managed.sol: Manages contract ownership and access.
Owned.sol: Ownership management.
helper/
MultiCallHelper.sol: Helper for multi-call functionalities.
storage/
IGuardianStorage.sol: Interface for guardian storage.
WalletFactory.sol: Factory for creating wallets.
zkSync/
facets/
Admin.sol: Admin functionalities.
Base.sol: Base contract for zkSync.
Executor.sol: Executes zkSync operations.
Getters.sol: Provides getters for zkSync.
Mailbox.sol: Mailbox for zkSync communication.
interfaces/
IAdmin.sol: Admin interface for zkSync.
IBase.sol: Base interface for zkSync.
IExecutor.sol: Executor interface for zkSync.
IGetters.sol: Getters interface for zkSync.
ILegacyGetters.sol: Legacy getters for zkSync.
IMailbox.sol: Mailbox interface for zkSync.
IVerifier.sol: Verifier interface for zkSync.
IZkSync.sol: zkSync interface.
libraries/
Diamond.sol: Diamond pattern implementation.
LibMap.sol: Map library for zkSync.
Merkle.sol: Merkle tree implementation.
PriorityQueue.sol: Priority queue for zkSync.
TransactionValidator.sol: Validates transactions.
Config.sol: Configuration for zkSync.
DiamondInit.sol: Initialization of Diamond pattern.
DiamondProxy.sol: Proxy implementation for Diamond pattern.
Storage.sol: Storage contract for zkSync.
ValidatorTimelock.sol: Timelock for validators.
Verifier.sol: Verifies zkSync transactions.
Additional Contracts
Counters.sol: Utility for counters.
HashStorage.sol: Stores hashes.
Upload.sol: Handles file uploads.
Messenger.sol: Messaging contract.
Structs.sol: Contains data structures.
MultiSigWallet.sol: Multi-signature wallet implementation.
Deployment Instructions
Set Up Environment: Ensure that you have the required tools and configurations. Install Truffle, Ganache, or other necessary tools.

Compile Contracts: Use Truffle or Hardhat to compile the smart contracts.


truffle compile
Deploy Contracts: Execute the deployment scripts. For example, using Truffle:


truffle migrate --network <network_name>
Verify Deployment: Ensure that the contracts have been correctly deployed to the specified network.

Interaction Instructions
Install Dependencies: Make sure all required dependencies are installed.


npm install
Set Up Web3: Configure Web3 or Ethers.js to interact with the contracts.

Interact with Contracts: Use the contract’s ABI and address to create an instance and call functions.


const contractInstance = new web3.eth.Contract(ABI, contractAddress);
contractInstance.methods.functionName(params).call();
Test Interactions: Write and run tests to ensure that interactions function as expected.

Contract Details
Identity Management
IdentityManagement.sol: Manages user identities.
Token Management
THETAStaking.sol: Implements staking mechanisms for THETA tokens.
Alvara Protocol
Alva.sol: Main contract for Alvara.
AlvaraGovernance.sol: Governance contract for Alvara.
AlvaraLending.sol: Lending functionality for Alvara.
AlvaraRewards.sol: Reward management for Alvara.
AlvaraStaking.sol: Staking functionality for Alvara.
AlvaraVault.sol: Vault for storing assets.
BTS.sol: BTS token contract.
BTSFactory.sol: Factory for creating BTS tokens.
BTSMarketplace.sol: Marketplace for BTS tokens.
BTSPair.sol: Token pair contract for BTS.
ERC-BTS.sol: ERC-BTS token standard implementation.
Factory.sol: Factory for Alvara-related contracts.
HiveX.sol: Marketplace and ecosystem integration.
Banking Integration
banking_contract.sol: Integrates banking functionalities.
BitTheta Secure
Analytics.sol: Provides analytics functionality.
RealTimeMonitoring.sol: Real-time monitoring services.
UsageAnalytics.sol: Usage analytics.
EscrowServices.sol: Escrow services.
OracleIntegration.sol: Integrates with oracles.
CommunityChannels.sol: Manages community channels.
SocialSharing.sol: Social sharing functionalities.
CrossChainTransfers.sol: Handles cross-chain transfers.
Interoperability.sol: Ensures interoperability.
EndToEndEncryption.sol: Provides end-to-end encryption.
Verifier.sol: Verifies encrypted data.
AchievementsBadges.sol: Manages achievements and badges.
ChallengesContests.sol: Handles challenges and contests.
DIDIntegration.sol: Integrates Decentralized Identifiers (DID).
ReputationSystem.sol: Manages reputation systems.
FileSharingIncentives.sol: Incentives for file sharing.
Staking.sol: Staking functionalities.
LiveStreaming.sol: Live streaming functionalities.
OnDemandContent.sol: On-demand content services.
Bridges
CrossChainToken.sol: Manages cross-chain tokens.
WormholeBridge.sol: Integrates Wormhole bridge.
Governance
Governance.sol: Governance contract.
IGovernance.sol: Governance interface.
SubchainGovernanceToken.sol: Token for governance.
Sustainability
eco_friendly_contract.sol: Contracts for eco-friendly initiatives.
Infrastructure
Managed.sol: Manages contract ownership and access.
Owned.sol: Ownership management.
MultiCallHelper.sol: Helper for multi-call functionalities.
IGuardianStorage.sol: Interface for guardian storage.
WalletFactory.sol: Factory for creating wallets.
zkSync
Admin.sol: Admin functionalities.
Base.sol: Base contract for zkSync.
Executor.sol: Executes zkSync operations.
Getters.sol: Provides getters for zkSync.
Mailbox.sol: Mailbox for zkSync communication.
IAdmin.sol: Admin interface for zkSync.
IBase.sol: Base interface for zkSync.
IExecutor.sol: Executor interface for zkSync.
IGetters.sol: Getters interface for zkSync.
ILegacyGetters.sol: Legacy getters for zkSync.
IMailbox.sol: Mailbox interface for zkSync.
IVerifier.sol: Verifier interface for zkSync.
IZkSync.sol: zkSync interface.
Diamond.sol: Diamond pattern implementation.
LibMap.sol: Map library for zkSync.
Merkle.sol: Merkle tree implementation.
PriorityQueue.sol: Priority queue for zkSync.
TransactionValidator.sol: Validates transactions.
Config.sol: Configuration for zkSync.
DiamondInit.sol: Initialization of Diamond pattern.
DiamondProxy.sol: Proxy implementation for Diamond pattern.
Storage.sol: Storage contract for zkSync.
ValidatorTimelock.sol: Timelock for validators.
Verifier.sol: Verifies zkSync transactions.
Additional Contracts
Counters.sol: Utility for counters.
HashStorage.sol: Stores hashes.
Upload.sol: Handles file uploads.
Messenger.sol: Messaging contract.
Structs.sol: Contains data structures.
MultiSigWallet.sol: Multi-signature wallet implementation.