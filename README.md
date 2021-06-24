## nano

[![CI](https://github.com/Oefenweb/ansible-nano/workflows/CI/badge.svg)](https://github.com/Oefenweb/ansible-nano/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-nano-blue.svg)](https://galaxy.ansible.com/Oefenweb/nano)

Set up nano in Debian-like systems.

#### Requirements

* `git` (will be installed)
* `make` (will be installed)

#### Variables

* `nano_nanorc_destinations` [default: `{skell: dest: /etc/skel, current: dest: "{{ ansible_env.HOME }}"}`]: Destinations to copy the nanorc file to
* `nano_nanorc_destinations.key`: The identifier of the file (e.g. `skel`)
* `nano_nanorc_destinations.key.dest`: The remote path of the file to copy (e.g. `/etc/skel`)
* `nano_nanorc_destinations.key.owner`: The name of the user that should own the file (optional, default `root`)
* `nano_nanorc_destinations.key.group`: The name of the group that should own the file (optional, default `owner`, then `root`)
* `nano_nanorc_destinations.key.mode`: The mode of the file, such as 0644 (optional, default `0644`)

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
