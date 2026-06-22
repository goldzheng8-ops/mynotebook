git config --global user.name "YourName"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
git config --global color.ui auto
ssh-keygen -t ed25519 -C "you@example.com"
Start-Service ssh-agent
ssh-add $env:USERPROFILE\.ssh\id_ed25519
type %USERPROFILE%\.ssh\id_ed25519.pub
git --version
ssh -T git@github.com
git config --global push.default simple
git config --global core.autocrlf true
git config --global credential.helper manager