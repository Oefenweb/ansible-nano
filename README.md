## nano [![Build Status](https://travis-ci.org/Oefenweb/ansible-nano.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-nano)

Set up nano in Debian-like systems.

#### Requirements

None

#### Variables

* `nano_nanorc_destinations`: [default: `[/etc/skel, {{ ansible_env.HOME }}]`]: Destinations to copy the nanorc file to
* `nano_tabsize`: [default: `2`]: Tab size
* `nano_tabstospaces`: [default: `true`]: Whether or not to convert typed tabs to spaces
* `nano_smooth_scrolling`: [default: `true`]: Whether or not to use smooth scrolling

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
