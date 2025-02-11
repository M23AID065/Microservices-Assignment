# VirtualBox VM Setup and Microservice Deployment

## Assignment Details
- **Name:** Ramaraju Venkata Veereswara Lohit
- **Roll No:** M23AID065

## Introduction
This project demonstrates the setup of Virtual Machines (VMs) using VirtualBox, network configuration, and deployment of a microservice-based application.

## Prerequisites
- VirtualBox Installed
- Ubuntu 20.04 or later VMs
- Node.js & MongoDB

## VM Setup & Network Configuration
1. Create two Virtual Machines:
   - **VM1 (API-backend Server)**
   - **VM2 (DB Server)**

2. Set up networking using Host-Only Adapter:
   - API-backend Server IP: `192.168.56.101`
   - DB Server IP: `192.168.56.102`

3. Enable SSH for remote access.

## Microservice Deployment
The API server is built with Node.js and connects to MongoDB running on the database server.

### Steps to Deploy:
1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the service:
   ```bash
   node server.js
   ```

## Docker Deployment
For containerized deployment, use:
```bash
docker-compose up -d
```

## Testing
Check API response:
```bash
curl http://192.168.56.101:5000/
```

