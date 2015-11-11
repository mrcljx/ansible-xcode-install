# xcversion (Ansible Module)

Wrapper around [NeoNacho](twitter.com/neonacho)'s [xcode-install](https://github.com/neonichu/xcode-install).

```
> XCVERSION

  Installs or selects a specified version of Xcode.

Options (= is mandatory):

- clean
        If `no', `xcode-install' won't remove the downloaded installation
        file to allow faster re-installation. (Choices: yes, no)

- password
        The password for `user' [Default: None]

- state
        indicate the desired state of the resource (Choices: present,
        selected) [Default: selected]

- user
        The Apple ID / e-mail for talking to Apple servers [Default: None]

= version
        version of Xcode to install/select

Requirements:  OS X, xcode-install Ruby Gem

EXAMPLES:
- name: Installs Xcode 7.1.1
  xcversion: state=present version=7.1.1

- name: Selects (and installs if necessary) Xcode 7.1.1
  xcversion: state=selected version=7.1.1


MAINTAINERS: Marcel Jackwerth (@sirlantis)
```
