# Ansible Role: gmrender-resurrect

An Ansible role that installs [gmrender-resurrect](https://github.com/hzeller/gmrender-resurrect) on Ubuntu/Debian.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

You have the choice to use some variables from the configuration:
```
gmrrs_outputpackagetype: alsa
gmrrs_sourcedir: /usr/src/gmrender-resurrect
gmrrs_description: "gmediarender-resurrect service"
gmrrs_user: gmrender-resurrect
gmrrs_group: audio
gmrrs_run: '/usr/local/bin/gmediarender --gstout-audiosink=alsasink --gstout-audiodevice=sysdefault --gstout-videosink=null -f "{{ inventory_hostname_short }}"'
```


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
- hosts: servers
  roles:
    - role: gmrender-resurrect
```

## License

Apache

## Author Information

Many thanks to:

* [HZeller](https://github.com/hzeller/gmrender-resurrect) who created this role
