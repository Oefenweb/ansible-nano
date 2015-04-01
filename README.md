## nano

[![Build Status](https://travis-ci.org/Oefenweb/ansible-nano.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-nano) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-nano-blue.svg)](https://galaxy.ansible.com/list#/roles/1499)

Set up nano in Debian-like systems.

#### Requirements

* `git-core` (will be installed)
* `make` (will be installed)

#### Variables

* `nano_nanorc_destinations`: [default: `[/etc/skel, {{ ansible_env.HOME }}]`]: Destinations to copy the nanorc file to
* `nano_tabsize`: [default: `2`]: Tab size
* `nano_tabstospaces`: [default: `true`]: Whether or not to convert typed tabs to spaces
* `nano_smooth_scrolling`: [default: `true`]: Whether or not to use smooth scrolling

* `nano_improved_nanorc_install`: [default: `true`]: Whether or not to install [improved syntax highlighting](https://github.com/nanorc/nanorc)
* `nano_improved_nanorc_langs`: [default: `all`]: Languages to enable after installation
* `nano_improved_nanorc_git_repo`: [default: `https://github.com/nanorc/nanorc`]: The repository url
* `nano_improved_nanorc_git_branch`: [default: `master`]: The branch to checkout

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - nano
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-nano/issues)!
