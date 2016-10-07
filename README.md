wrboyce.dotfiles-vim
====================

[![Build Status](https://travis-ci.org/wrboyce/ansible-dotfiles-vim.svg)](https://travis-ci.org/wrboyce/ansible-dotfiles-vim)

Configure vimrc via custom repo

Requirements
------------

Depends on the `user_home` and `user_usernames` variables being set.

Role Variables
--------------

Custom repo defaults to `https://github.com/{{ user_username }}/vimrc.git`, variable `user_username` or
`vim_vimrc_repo` must be set.

Example Playbook
----------------

    - hosts: workstations
      roles:
         - wrboyce.dotfiles-vim

License
-------

Apache 2.0
