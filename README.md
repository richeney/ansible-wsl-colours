# Installs Packer

Ansible role to download Packer on Ubuntu 16.04 (xenial), 18.04 (bionic) or 20.04 (focal).


The Hashicorp releases API will be queried for the latest stable Packer binary.

The binary will then be downloaded to /usr/local/bin retaining the version number.

A /usr/local/bin/terraform symbolic link will point at the latest binary.


## Installation

`ansible-galaxy install richeney.packer`

## Example Playbook

```yaml
- hosts: all
  roles:
    - richeney.packer
```

## Requirements

None.

## Dependencies

The zip package will be installed if not present.
