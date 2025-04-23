# Aggregata Session Manager

## What is Aggregata?

Aggregata is a decentralized data generation and validation protocol developed by Gata.xyz. It leverages community participation to create and curate high-quality datasets used to train state-of-the-art AI models, particularly in the field of vision-language understanding. Through the Aggregata platform, users can engage in tasks like validating image-caption pairs, helping ensure that the data used in AI training is accurate, diverse, and human-aligned. By incentivizing contributions through token rewards, Aggregata aims to democratize the data supply chain for frontier artificial intelligence systems.

## Description
The Aggregata Session Manager is a utility designed to manage authenticated interactions across multiple user sessions within a web-based dashboard. It automates session initiation, navigates to task-specific interfaces, and executes predefined workflows. Designed for scalability, it supports multi-account environments and proxy routing for distributed operations.

## Features
- **Multi-Session Management**: Automates execution across several authenticated sessions.
- **Workflow Execution**: Navigates through interfaces and initiates workflows autonomously.
- **Proxy Support**: Supports proxy rotation per session to ensure distributed request patterns.
- **Debugging Tools**: Captures screenshots and logs for traceability and troubleshooting.

## Prerequisites
- Node.js
- Playwright:
  ```bash
  npm install playwright
  ```

## Required File Structure
- `accounts.json`: Array of session profiles containing credentials and access tokens.
- `proxies.txt`: (Optional) List of proxies in the format `http://username:password@ip:port`.

## Setup and Execution

### Setup
```bash
git clone https://github.com/SEU-USUARIO/Aggregata-Workflow-Executor.git
cd Aggregata-Workflow-Executor
npm install
```

Configure `accounts.json` and (optionally) `proxies.txt`.

### Running the Executor
```bash
node index.js
```

You will be prompted to choose whether to use proxies. The executor will then run all session tasks accordingly, logging outputs and saving screenshots for verification.

## License
Distributed under the MIT license.

## Contributions
Contributions are welcome via pull request.
