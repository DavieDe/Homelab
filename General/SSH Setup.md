# SSH Documentation

- The SSH agent needs to be started in the background
- eval "$(ssh-agent -s)"
- ssh-add ~/.ssh/(key) 
- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent
- Test connection ssh -T git@github.com
- Add script to .bashrc
- if [ -z "$SSH_AUTH_SOCK" ] ; then
  eval `ssh-agent -s`
  ssh-add ~/.ssh/id_rsa(key file)
fi
- This will only add the specified key and start the agent on startup. If other keys need to be added add with ssh-add ~/.ssh/(key)