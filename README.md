# Ansible role to Github GIT LFS

Installs Git LFS, "an open source Git extension for versioning large files", on any RHEL/CentOS or Debian/Ubuntu Linux system. Source of packages is [package cloud](https://packagecloud.io/github/git-lfs/)

![Build Status](https://travis-ci.org/pedrocarmona/github-git-lfs.svg?branch=master)

Sponsored by [BidMath](http://bidmath.com/)

## Requirements

- { role: pedrocarmona.github-git-lfs }

It depends on ansible 2.1, for earlier versions, please checkout this [tag](https://github.com/BidMath/github-git-lfs/releases/tag/v1.2.0)

## Example Playbook

```yaml
- hosts: servers
  roles:
    - { role: pedrocarmona.github-git-lfs }
```


## License

MIT / BSD
