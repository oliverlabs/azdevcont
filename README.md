# Custom GitHub Codespaces Container with Azure CLI, Bicep and Terraform

This is my implementation of a GitHub devcontainer with Az CLI, Bicep, Terraform and a few other components pre-installed. It is based on the Azure Bicep Community devcontainer.

You can use it in GitHub Codespaces or locally as a devcontainer.

## Try It Out

Often times the deployment process for many repos uses a concept of *Developing inside a Container* to containerize all the necessary pre-requisite component without requiring them to be installed on the local machine. This is where this template can be useful. The environment you will work in will be created using a development container, or dev container hosted on a virtual machine using GitHub Codespaces.

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/oliverlabs/azdevcont) <br>
[![Open in VS Code Dev Containers](https://img.shields.io/static/v1?style=for-the-badge&label=VSCode%20-%20DevContainer&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/oliverlabs/azdevcont)
[![Open in VS Code - Insiders Dev Containers](https://img.shields.io/static/v1?style=for-the-badge&label=VSCode-Insiders%20-%20Devcontainer&message=Open&color=blue&logo=visualstudiocode)](https://insiders.vscode.dev/redirect?url=vscode-insiders://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/oliverlabs/azdevcont)

> [!NOTE]  
> More information can be found at [Developing inside a Container](https://code.visualstudio.com/docs/remote/containers).

## What's Available?

Here is a list of tools that are available out-the-box with this Codespaces container:

- Linux Ubuntu Noble Numbat (LTS-24.04) used as a base image
- zsh Linux shell as default (bash is available)
- oh-my-zsh extension for zsh with the legendary STARSHIP theme
- Azure CLI
- Azure Developer CLI (azd)
- Docker in Docker
- Dotnet Runtime
- GitHub CLI
- Azure Bicep CLI
- jq tool (lightweight and flexible command-line JSON processor)
- Terraform
- python3
- Node
- Helm
- Minikube
- Kubectl
- sshd

Please note that, if available, the *latest* version of the package is used.

## VS Code Extensions

- GitHub Actions
- Azure CLI
- VS Code dotnet runtime
- VS Code Bicep
- Material Icon Theme
- azurerm-vscode-tools
- ms-azuretools.vscode-docker
- draw.io integration
- scroll-back history for terminal: 1,000,000 lines
- UK Keyboard layout for browser based GitHub Codespaces as default

## Remoting Into Codespaces
You can remote into the created Codespaces from your local machine using ssh. Refer to the commands [here](https://docs.github.com/en/codespaces/developing-in-a-codespace/using-github-codespaces-with-github-cli).

Example:
```bash
gh cs ssh -c [CODESPACENAME]
```
Once connected, you can type `zsh` to use the zsh shell.

Happy coding!
