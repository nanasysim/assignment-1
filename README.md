# Guide to Setting Up and Managing DigitalOcean with doctl and cloud-init

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Install doctl](#1-install-doctl)
4. [Create an API Token in DigitalOcean](#2-create-an-api-token-in-digitalocean)

## Introduction
Before you set up your DigitalOcean with doctl, you must have a basic understanding of what those are. 

### What is doctl?
* Open-source command-line interface (CLI) tool
* Available as precompiled binary for Linux, macOS, and Windows
* Saves time when managing resources in DigitalOcean accounts
* Simplifies more comple workflows and activities
* Provides full API access to DigitalOcean, allowing you to create, configure, and destroy resources like Droplets, Kubernetes clusters, firewalls, load balancers, database clusters, domains, and more

### What is DigitalOcean?
* Offers a range of cloud services to help developers and businesses deploy, manage, and scale application
* Provides virtual machines (droplets), which can be used to host websites, applications, and other services

### Why use doctl to Set up and Manage DigitalOcean?
* doctl allows you to interact with DigitalOcean via the command line
* doctl supprots all functionalities found in the DigitalOcean control panel
* Enables you to create, configure, and destroy DigitalOcean resources like Droplets, Kubernetes clusters, firewalls, load balancers, database clusters, domains, and more

## Prerequisites
* A DigitalOcean account
* A GitHub account
* An Arch Linux Droplet

Now that you know some general information and the prerequisites, let's get started.

## 1. Install doctl
Before you set up your DigitalOcean, you must make sure that you have doctl successfully installed on your computer. 

### Step 1: Run this command to download the latest version of doctl
```sudo pacman -S doctl``` 
* This command installs doctl on Arch Linux

**This is how it looks on the Terminal:**  

![sudo-pacman-doctl](assets/sudo-pacman-doctl.png)

### Step 2: Verify that doctl is installed by running this command
```doctl version```
* This command checks the version of doctl installed on your computer

**This is how it looks on the Terminal:** 

![doctl-version](assets/doctl-version.png)

Now that you have doctl installed, you can proceed to set up your DigitalOcean account.

## 2. Create an API Token in DigitalOcean
Before you can use doctl to manage your DigitalOcean resources, you need to create an API token in DigitalOcean. This token will allow you to authenticate your doctl commands with DigitalOcean.

### What is an API Token?
* Unique identifier used to authenticate a user, developer, or application when interacting with an API
* Think of it like a digital key that grants access to specific resources or actions provided by the API

### Why do you need an API Token?
* Required to authenticate your doctl commands with DigitalOcean
* Ensures only authorized users can access and manage your DigitalOcean resources
* Can be configured with specific permissions to restrict access to certain resources or actions
* Help track usage and monitor activity
* Simplify the authentication process 

Now let's create an API token in DigitalOcean.

