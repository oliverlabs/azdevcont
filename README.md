# Custom GitHub Codespaces Container with Azure CLI, Bicep and Terraform 
This is my implementation of a GitHub devcontainer with Az CLI, Bicep, Terraform and a few other components pre-installed. It is based on the Azure Bicep Community devcontainer.

You can use it in GitHub Codespaces or locally as a devcontainer.

# What's Available?
Here is a list of tools that are available out-the-box with this Codespaces container:

- Linux Ubuntu Jammy (LTS-22.04) used as a base image
- zsh Linux shell as default (bash is available)
- oh-my-zsh extension for zsh with the legendary STARSHIP theme
- Azure CLI 
- GitHub CLI
- Azure Bicep CLI
- jq tool (lightweight and flexible command-line JSON processor)
- Terraform 
- python3
- Node 
- Helm 
- Minikube
- Kubectl

Please note that, if available, the _latest_ version of the package is used.

## VS Code Extensions
- GitHub Actions
- Azure CLI
- VS Code dotnet runtime
- VS Code Bicep
- Material Icon Theme
- azurerm-vscode-tools
- ms-azuretools.vscode-docker
- scroll-back history for terminal: 1,000,000 lines
- UK Keyboard layout for browser based GitHub Codespaces as default
