# AgneaX OS Official APT Repository

This repository hosts official software updates, security patches, and application packages for **AgneaX OS (Ubuntu 24.04 LTS noble)**.

## Adding to AgneaX OS / Ubuntu

```bash
# 1. Install AgneaX Archive Keyring
sudo wget -O /usr/share/keyrings/agneax-archive-keyring.gpg https://agneax.github.io/apt-repo/agneax-archive-keyring.gpg

# 2. Add the APT source
sudo tee /etc/apt/sources.list.d/agneax.sources << 'EOF'
Types: deb
URIs: https://agneax.github.io/apt-repo/
Suites: noble
Components: main
Architectures: amd64
Signed-By: /usr/share/keyrings/agneax-archive-keyring.gpg
EOF

# 3. Update and upgrade
sudo apt update && sudo apt upgrade
```
