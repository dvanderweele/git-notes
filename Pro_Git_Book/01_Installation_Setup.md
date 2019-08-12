# Installation & Setup

On a red hat distro, the command to install git:
```bash
sudo dnf install git-all
```
On a debian distro like ubuntu, the command to install git:
```bash
sudo apt install git-all
```
A command to show all of your git settings and where they are coming from:
```bash
git config --list --show-origin
```
A command to set your user name, typically done after installing git:
```bash 
git config --global user.name "John Doe"
```
A command to set your email address, typically done after installing git:
```bash
git config --global user.email johndoe@example.com
```
A command to set the default text editor that git will try to open if it, say, needs you to type a message:
```bash 
git config --global core.editor nano
```

