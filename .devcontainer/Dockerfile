# [Choice] .NET Core version: 3.1, 2.1
ARG VARIANT=3.1
FROM mcr.microsoft.com/devcontainers/dotnet:0-3.1

COPY library-scripts/azcli-debian.sh /tmp/library-scripts/
COPY library-scripts/common-debian.sh /tmp/library-scripts/

RUN bash /tmp/library-scripts/azcli-debian.sh \
    && curl -Lo /usr/local/bin/bicep https://github.com/Azure/bicep/releases/latest/download/bicep-linux-x64 \
    && chmod +x /usr/local/bin/bicep \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/* /tmp/library-scripts \
    && curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl" \
    && sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl 
    # && curl -fsSL https://get.docker.com | bash

# RUN bash /tmp/library-scripts/common-debian.sh "false" "olivergulich" "automatic" "automatic" "true" "false"

RUN az bicep install
RUN export PATH=/home/vscode/.azure/bin/bicep:$PATH
    
RUN /bin/zsh
# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends kubectl
