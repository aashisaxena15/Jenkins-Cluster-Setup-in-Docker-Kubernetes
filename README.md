# 🚀 Jenkins Cluster from Scratch Using Docker & Kubernetes

CHECK OUT THE MEDIUM BLOG FOR THE DETAILED EXPLANATION: https://aashisaxena15.medium.com/jenkins-cluster-setup-in-docker-kubernetes-569aa19e6b4f

This project provides a hands-on, step-by-step guide to manually build a Jenkins master-agent architecture using Docker containers and scale it on Kubernetes using custom-built Jenkins images — without relying on any prebuilt Jenkins images.

---

## 📚 Table of Contents

- [Project Overview](#project-overview)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Phase 1: Jenkins Cluster on Docker](#phase-1-jenkins-cluster-on-docker)
- [Phase 2: Jenkins Cluster on Kubernetes](#phase-2-jenkins-cluster-on-kubernetes)
- [SSH Agent Configuration](#ssh-agent-configuration)
- [Sample Pipeline](#sample-pipeline)
- [Folder Structure](#folder-structure)

---

## 📌 Project Overview

- Manual installation of Jenkins on Ubuntu-based Docker containers
- Custom Dockerfiles to build Jenkins master and agent images
- Kubernetes deployments for Jenkins master and agents
- SSH-based secure agent communication
- Docker build & deployment pipeline as a CI/CD example

---

## 🧱 Architecture

The architecture consists of two phases:

1. **Docker Environment:**
   - Jenkins Master and Agent as Docker containers
   - Manual Java and Jenkins installation
   - Agent connected via JNLP

2. **Kubernetes Environment:**
   - Custom Jenkins Master & Agent images
   - YAML deployments for production-scale orchestration
   - SSH-based agent connection
   - NodePort exposed Jenkins Web UI

![Architecture](./assets/jenkins-architecture.png)

---

## ⚙️ Tech Stack

- Jenkins (WAR-based setup)
- Docker (Manual container setup)
- Kubernetes (Deployments, Services)
- Ubuntu 22.04 (Base image)
- Red Hat UBI9 (For agent image)
- Java (OpenJDK 17 & 21)
- Git, curl, wget, OpenSSH

---
