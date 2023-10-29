# SOPS Setup

- https://blog.gitguardian.com/a-comprehensive-guide-to-sops/

## Install SOPS

- Download from <https://github.com/getsops/sops/releases>
- Follow the installation (Use Brew install sops)

- install gnupg

## How to use
- make sure the .sops.yaml file is in the root of the repo
- to encrypt before commiting use sops -i e (file name)
- to decrypt after commiting use sops -i -d (file name)