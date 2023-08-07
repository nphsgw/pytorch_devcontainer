# PyTorch Development Environment with VS Code and DevContainer

This template enables quick setup of a PyTorch development environment using VS Code and DevContainer.

## Features

- **VS Code and DevContainer Integration**: Code directly in a Docker container with VS Code's Remote - Containers extension.
- **Pre-installed PyTorch**: No need for manual setup; PyTorch and its dependencies are ready to use.

## Requirements

- [VS Code](https://code.visualstudio.com/)
- [Docker](https://www.docker.com/)
- [Remote - Containers VSCode Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- [NVIDIA driver](https://docs.nvidia.com/datacenter/tesla/tesla-installation-notes/index.html)
- [NVIDIA Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html)

## Usage

1. Click on the `Use this template` button to create a new project based on this template, or clone this project using `git clone`.

2. Clone the project you created in step 1 to your local environment and open it in VS Code.

3. If you have DevContainer installed, click on the `Reopen in container` message that appears.

4. If the icon in the lower left corner of the VS Code screen becomes `DevContainer:pytorch`, you have successfully set up the environment. Please confirm that CUDA is available in `sample.ipynb`.

## Customizing the Environment

This project includes a `devcontainer.json` file and a `Dockerfile`. You can modify these files to customize the development environment according to your needs.

- **devcontainer.json**: This file contains settings for the VS Code DevContainer. You can specify the Dockerfile, set forward ports, set post-create commands, and more.

- **Dockerfile**: This file defines the Docker container. You can add or remove software, libraries, or tools that are installed in the container.
