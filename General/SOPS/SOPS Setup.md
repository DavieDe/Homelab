# SOPS Setup

- https://blog.gitguardian.com/a-comprehensive-guide-to-sops/
- https://www.youtube.com/watch?v=1BquzE3Yb4I

## Install SOPS

- SOPS will allow us to encrypt and decrypt our secrets

- Download from <https://github.com/getsops/sops/releases>
- Follow the installation (Use Brew install sops)

## Install Age
- Age is what creates the encryption
- install age
- Have Age generate the key 
    - age-keygen -o keys.txt
- Move this keys.txt to ~/.config/sops/age/keys.txt
- You can share this file to another machine so it can also encrypt and decrypt files

## How to use
- make sure the .sops.yaml file is in the root of the repo
    - The .sops.yaml file should contain creation_rules then rules for age (The public key)

# Commands
- to encrypt before commiting use sops -i e (file name)
- to decrypt after pulling use sops -i -d (file name)