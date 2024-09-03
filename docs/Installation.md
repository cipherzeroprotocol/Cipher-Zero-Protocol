# Installation Guide

Welcome to the BitTheta Secure project! This guide will walk you through setting up and running the project on your local machine.

## Prerequisites

Before you begin, make sure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (v14.x or later)
- [Yarn](https://yarnpkg.com/) (v1.x or later)
- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/get-started) (optional, for running certain services)
- [Go](https://golang.org/dl/) (v1.14.1 or later)
- [Python](https://www.python.org/downloads/) (v3.x or later)
- [Solidity](https://docs.soliditylang.org/en/latest/installing-solidity.html)
- [TypeScript](https://www.typescriptlang.org/download)


## Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/arhansuba/bitthetasecure.git
cd BitThetaSecure
Project Structure
Here is an overview of the project structure:


.vscode
BitThetaCLI
ai
backend
circom
contracts
docs
frontend
ignition
integration_scripts
interoperability
migrations
privacy
scripts
sdk
services
user_interface
utils
.gitattributes
.gitignore
README.md
challenge_0003
circuit.circom
go1.14.1.linux-amd64.tar.gz
hardhat.config.js
package-lock.json
package.json
pot14_0000.ptau
pot14_0001.ptau
pot14_0002.ptau
pot14_0003.ptau
pot14_beacon.ptau
pot14_final.ptau
response_0003
soljson-v0.8.7+commit.e28d00a7.js
truffle-config.js
yarn.lock

Install Dependencies
Navigate to the project root and install the dependencies:


yarn install
Environment Variables
Create a .env file in the project root directory and add the necessary environment variables. Refer to the .env.example file for the required variables.

Compile Contracts
Compile the smart contracts using Truffle:


yarn truffle compile
Migrate Contracts
Migrate the smart contracts to your local blockchain:


yarn truffle migrate
Running the Backend
Navigate to the backend directory and start the backend services:


cd backend
yarn install
yarn start

Running the Frontend
Navigate to the frontend directory and start the frontend application:


cd frontend
yarn install
yarn start
Running Other Services
You may need to start additional services depending on the features you want to use. Refer to the individual service directories (services, integration_scripts, privacy, etc.) for specific instructions.



Docker
If you are using Docker to run certain services, make sure to follow the instructions in the respective directories for setting up Docker containers.

Go
To install Go, use the provided tarball:


tar -xvf go1.14.1.linux-amd64.tar.gz
sudo mv go /usr/local
Add the Go binary to your PATH:


export PATH=$PATH:/usr/local/go/bin
Troubleshooting
If you encounter any issues, check the following:

Ensure all dependencies are installed correctly.
Make sure your environment variables are set up correctly.
Check the logs for any error messages.
For further assistance, feel free to open an issue on the GitHub repository.

Thank you for contributing to BitTheta Secure! We appreciate your efforts to make this project better.


