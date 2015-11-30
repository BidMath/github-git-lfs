# Ansible role to Github GIT LFS

Installs Git LFS, a distributed version control system, on any RHEL/CentOS or Debian/Ubuntu Linux system. Source of packages is [package cloud](https://packagecloud.io/github/git-lfs/)

## Requirements

- { role: pedrocarmona.github-git-lfs }

## Example Playbook

    - hosts: servers
      roles:
        - { role: pedrocarmona.github-git-lfs }

## License

MIT / BSD
