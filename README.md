# WIN dev Docker recipe 
*A recipe to develop with Docker on Windows without headaches.*

## Table of Contents
- [WIN dev Docker recipe](#win-dev-docker-recipe)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)

---

## Introduction
Developing with Docker on Windows can sometimes be challenging due to compatibility issues or misconfigurations. This guide provides a streamlined setup to avoid common pitfalls and ensure a smooth development experience.

## Prerequisites
Before starting, make sure you have the following installed on your system:
- **Windows 10/11 Pro or Enterprise** (with WSL2 enabled)
- [Docker Desktop for Windows](https://www.docker.com/products/docker-desktop)
- [Windows Subsystem for Linux (WSL2)](https://learn.microsoft.com/en-us/windows/wsl/)
- A preferred Linux distribution installed via WSL2 (e.g., Ubuntu)

## Setup
1. **Enable WSL2 Integration**:
   - Open Docker Desktop and navigate to *Settings > Resources > WSL Integration*.
   - Enable integration with your preferred Linux distribution.

2. **Install Docker in WSL2**:
   Open your WSL2 terminal and run the following commands:
   ```bash
   sudo apt update
   sudo apt install docker.io
   sudo usermod -aG docker $USER
