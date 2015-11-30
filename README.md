# Ansible role to Github GIT LFS

Installs Git LFS, "an open source Git extension for versioning large files", on any RHEL/CentOS or Debian/Ubuntu Linux system. Source of packages is [package cloud](https://packagecloud.io/github/git-lfs/)

![Build Status](https://travis-ci.org/pedrocarmona/github-git-lfs.svg?branch=master)

## Requirements

- { role: pedrocarmona.github-git-lfs }

## Example Playbook

```yaml
- hosts: servers
  roles:
    - { role: pedrocarmona.github-git-lfs }
```


## Usage notes

Added the git_lfs_install_vars variable to defaults, in order to provide the ability to not download files in LFS when you clone the repo. Currently is faster to clone a repo and then use git lfs pull, because git lfs pull has better implementation on download:

```yaml

- hosts: servers
  roles:
    - { role: pedrocarmona.github-git-lfs }
  tasks:
    - git: >
      repo=git://foosball.example.org/path/to/repo.git
      dest=repodir/

    - command: git lfs pull
      args:
        chdir: repodir/
```


## License

MIT / BSD
