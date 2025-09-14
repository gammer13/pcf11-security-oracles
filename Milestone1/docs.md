# Security Oracles – User Guide

## Overview

This User Guide provides step-by-step instructions and background information for setting up and using the Security Oracles framework on Cardano. It combines research insights with practical deployment scripts.

The guide is divided into:

- Understanding Security Oracles
- System Setup
- Using Transaction & Utility Scripts
- Best Practices & Governance Models

---

## 1. Understanding Security Oracles

### What are Security Oracles?

Security Oracles provide Cardano smart contracts with the ability to adapt their execution in response to real-time threats.

### Threat Detection Approach

- **Community Staked Detection Network** → Decentralized, staked operators running detection bots.  
- **Oracle Attestation Layer** → Signed threat scores via oracle feeds.  
- **Treasury-Funded Watch-Dog Service** → DAO-funded central analytics.  

### Governance & Funding Options

- **M1 –** Treasury Grants & DAO Bounties  
- **M2 –** Work-Token Staking Network  
- **M3 –** Pay-per-Trigger Service Fee  
- **M4 –** Enterprise SaaS with Insurance  

---

## 2. System Setup

### Prerequisites

Install and configure the following:

- `cardano-node v10.1.3`
- `nix` package manager
- `hydra` (version 0.20.0)

Set `REPO_HOME` in `/scripts/env.sh`.

### Initial Setup

```bash
cd scripts
chmod +x 00-setup.sh
./00-setup.sh
