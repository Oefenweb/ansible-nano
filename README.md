## nano [![Build Status](https://travis-ci.org/Oefenweb/ansible-nano.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-nano)

Set up nano in Debian-like systems.

#### Requirements

None

#### Variables

* `nano_nanorc_destinations`: [default: `[/etc/skel, {{ ansible_env.HOME }}]`]: Destinations to copy the nanorc file to
* `nano_tabsize`: [default: `2`]: Use this tab size instead of the default
* `nano_tabstospaces`: [default: `true`]: Convert typed tabs to spaces

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
