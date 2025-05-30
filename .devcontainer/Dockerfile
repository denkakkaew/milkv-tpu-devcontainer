FROM sophgo/tpuc_dev:v3.1

# Set the working directory
WORKDIR /workspace

# Create group and user 'vscode' with UID and GID 1000
RUN groupadd -g 1000 vscode && \
    useradd -m -u 1000 -g 1000 -s /bin/bash vscode && \
    apt-get update && \
    apt-get install -y sudo && \
    echo "vscode ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER vscode