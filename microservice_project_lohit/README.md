# VirtualBox VM Setup and Microservice Deployment

## Assignment Details:
- **Name:** Ramaraju Venkata Veereswara Lohit
- **Roll No:** M23AID065

## Introduction
This project involves setting up multiple virtual machines (VMs) using VMware, configuring networking between them, and deploying a microservice-based application.

## Prerequisites
- VMware Workstation
- Ubuntu Server ISO
- Basic knowledge of Linux commands

## Installation Steps

### 1. Install VMware
Download and install VMware Workstation from the official website.

### 2. Create Virtual Machines
- Create two VMs: `VM1` (API-Server) with IP address : 10.0.2.15 and `VM2` (DB-Server).
- Assign static IPs to each VM.

### 3. Configure Network Between VMs
- Set up a **Host-Only Adapter** network in VMware.
- Use `netplan` to configure static IPs for both VMs.

### 4. Deploy the Microservice
- Install Node.js and MongoDB on respective VMs.
- Clone the project repository and run the server.

## Repository Structure
```
/microservice-project
│── API_ServerFile/
│── DB_ServerFile/
│── node_modules/
│── README.md
│── package.json
│── package-lock.json
```

## Testing & Validation
- Use `curl` to verify API responses.
- Connect to the database from the API server.

