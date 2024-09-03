# Frontend Developer Guide

This document provides an overview of the frontend codebase for the BitTheta Secure project, detailing the structure and components to help developers understand and navigate the code effectively.

## Table of Contents

1. [Codebase Structure](#codebase-structure)
2. [Core Components](#core-components)
3. [Key Directories and Files](#key-directories-and-files)
4. [Configuration and Integration](#configuration-and-integration)
5. [Development and Testing](#development-and-testing)
6. [Best Practices](#best-practices)

## Codebase Structure

The frontend codebase is organized into a modular structure to support various functionalities of the BitTheta Secure platform. The main directories and their purposes are as follows:

- **`lib/`**: Contains helper functions and utilities.
- **`public/`**: Holds static assets and public resources.
- **`src/`**: Contains the core source code, including components, services, and contexts.
- **`config/`**: Includes configuration files for different services and environments.
- **`integration/`**: Handles integration scripts and configurations for various protocols and services.
- **`pages/`**: Defines different pages and views within the application.
- **`styles/`**: Contains stylesheets and style-related files.
- **`utils/`**: Includes utility functions and helpers.

## Core Components

### `src/components/`

The `components/` directory contains reusable UI components categorized by their functionalities:

- **`AI/`**: Components related to AI functionalities.
- **`Core/`**: Core components like headers, footers, and layout elements.
- **`FileStorage/`**: Components for file storage and management.
- **`IdentityManagement/`**: Components for managing user identities.
- **`MediaFeatures/`**: Components for media-related features like photo and video transfer.
- **`TokenManagement/`**: Components for managing tokens and related functionalities.
- **`UploadBox/`**: Components for file upload interfaces.

### `src/sections/`

This directory contains components that represent distinct sections of the application:

- **`ConnectWallet.tsx`**: Interface for connecting user wallets.
- **`Delivery.jsx`**: Components related to content delivery.
- **`Encryption.jsx`**: Components for encryption functionalities.
- **`FileMailer.js`**: Component for file mailing features.
- **`HomeDash.js`**: Dashboard for the home view.
- **`PhotoTransfer.tsx`**: Interface for photo transfer functionalities.
- **`Storage.tsx`**: Components for storage management.
- **`VideoTransfer.tsx`**: Interface for video transfer functionalities.

### `src/contexts/`

Defines React contexts used for state management and providing global data:

- **`AuthContext.tsx`**: Manages authentication state and user information.
- **`ConfigContext.tsx`**: Provides configuration settings throughout the application.
- **`DeliveryContext.tsx`**: Manages delivery-related state.
- **`ThetaContext.tsx`**: Handles state and data related to the Theta Network.

### `src/services/`

Contains service files for interacting with APIs and managing business logic:

- **`FileStorage.tsx`**: Manages file storage services.
- **`VideoService.ts`**: Handles video-related services.
- **`WalletService.ts`**: Manages wallet connections and transactions.
- **`CrossChainService.ts`**: Handles cross-chain communication services.

## Key Directories and Files

### `lib/`

Contains helper functions and utilities:

- **`apiHelper.ts`**: Functions for API interactions.
- **`dataHelper.ts`**: Helpers for data manipulation.
- **`cryptoUtils.ts`**: Utility functions for cryptographic operations.
- **`formatUtils.ts`**: Functions for data formatting.

### `config/`

Configuration files for various services and environments:

- **`BridgeConfig.ts`**: Configuration for cross-chain bridging.
- **`NetworkConfig.ts`**: Settings related to network configurations.
- **`sdkConfig.js`**: Configuration for SDK integrations.

### `pages/`

Defines the main pages and routing for the application:

- **`404.tsx`**: Custom 404 error page.
- **`index.tsx`**: The main entry point for the application.
- **`Home.tsx`**: Home page component.
- **`Content.tsx`**: Page for content-related functionalities.

### `styles/`

Stylesheets and style-related files:

- **`components.css`**: Styles for various components.
- **`globals.css`**: Global styles applied across the application.
- **`styles.scss`**: SCSS files for advanced styling.

## Configuration and Integration

### Environment Variables

Ensure environment variables are set up correctly for different environments. Use the `.env` file to manage sensitive information such as API keys and configuration settings.

### Integration Scripts

Scripts for integrating various protocols and services are located in the `integration_scripts/` directory:

- **`algorithmic_coin_integration.js`**: Integration for algorithmic coin functionalities.
- **`cross_border_payment_integration.js`**: Handles cross-border payment integrations.
- **`tokenized_assets_integration.js`**: Manages integration for tokenized assets.

### Contract Configurations

Smart contract configurations are managed in the `config/` directory:

- **`DIDContractABI.ts`**: ABI for the DID contract.
- **`IdentityContractABI.ts`**: ABI for the Identity contract.

## Development and Testing

### Running the Development Server

To start the development server, use the following command:

```bash
npm start
