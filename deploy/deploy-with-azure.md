---
if: visitor.claims.isAlphaUser
---

# Deploy with Azure

## Deploying Rocket.Chat on Azure

Deploying Rocket.Chat on Azure involves several key steps to ensure a successful setup. Follow this guide to get started.

### Prerequisites

* An active Azure account
* Basic knowledge of Azure services and virtual machines
* SSH client installed on your local machine

### Steps to Deploy Rocket.Chat

#### Step 1: Create an Azure VM

1. Navigate to the Azure Portal and select **Create a resource** > **Virtual Machine**.
2. Fill out the necessary details:
   * **Resource Group**: Select or create a new one.
   * **VM Name**: Enter a name for your VM.
   * **Region**: Choose the closest region.
   * **Image**: Select an appropriate Linux distribution (e.g., Ubuntu Server).
   * **Size**: Pick a size based on your requirements.
3. Configure **Administrator Account** with SSH public key for access.
4. Allow inbound ports: HTTP (80), HTTPS (443), and SSH (22).

#### Step 2: Install Rocket.Chat

1.  SSH into your VM:

    ```bash
    ssh <username>@<your_vm_public_ip>
    2
    ```
