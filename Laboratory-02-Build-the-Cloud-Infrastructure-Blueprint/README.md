# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory focused on investigating a cloud-based Linux server and understanding the basic components of cloud infrastructure. The KillerCoda Playground was used to inspect the server and document its resources before designing a simple cloud infrastructure.

## Objectives

- Identify the major components of cloud infrastructure.
- Investigate the resources available in a Linux environment.
- Understand compute, storage, networking, and operating system resources.
- Compare the core services of major cloud providers.
- Create a simple cloud infrastructure diagram.
- Document the investigation using Markdown.

## Cloud Infrastructure Components

The main cloud infrastructure components identified were:

- **Compute:** Intel Xeon E312xx CPU with 1 CPU core.
- **Storage:** 19G disk used to store the Linux system and files.
- **Networking:** IP addresses used to provide network connectivity.
- **Operating System:** Ubuntu 24.04.4 LTS, which manages the server resources and provides the environment for running commands and applications.

## Tools Used

- KillerCoda Playground
- Ubuntu Linux
- GitHub
- Markdown
- Draw.io / Diagramming Tool
- Web Browser

## Linux Commands Executed

The following commands were used to investigate the Linux environment:

```bash
cat /etc/os-release
uname -r
lscpu | grep "Model name"
nproc
free -h
df -h
hostname
hostname -I
