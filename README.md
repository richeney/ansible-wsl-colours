# Set vi and ls colours in a Windows System for Linux (WSL) Ubuntu environment.

Ansible role to set the colours for either Ubuntu 16.04 (xenial), 18.04 (bionic) or 20.04 (focal).

Creates and configures the following in the user's home directory:

* .vimrc
* .vim/colors/cloudshell.vim
* .dircolors

## Installation

`ansible-galaxy install richeney.wsl_colours`

## Example Playbook

```yaml
- hosts: all
  roles:
    - richeney.wsl_colours
```

## Requirements

None.

## Warning

Will automatically set the user and group to the ansible_user. WSL creates a user and sets the primary group to the same name.

## Dependencies

None.
