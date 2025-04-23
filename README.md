# Aggregata Workflow Executor

## Description
The Aggregata Workflow Executor is a utility designed to manage authenticated interactions across multiple user sessions within a web-based dashboard. It automates session initiation, navigates to task-specific interfaces, and executes predefined workflows. Designed for scalability, it supports multi-account environments and proxy routing for distributed operations.

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
