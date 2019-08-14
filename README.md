# Mac Development Ansible Playbook

This repository is a fork of Jeff Geerlings excellent repository: https://github.com/geerlingguy/mac-dev-playbook
It is a stripped version suited to my needs.

For installation:

    $ cd /usr/local
    $ sudo chown -R <your-username>:staff *
    $ xcode-select --install
    $ sudo easy_install pip
    $ sudo pip install ansible
    $ mkdir dev && cd dev
    $ git clone git@github.com:philippschreiber/mac-dev-playbook.git
    $ cd mac-dev-playbook
    $ ansible-galaxy install -r requirements.yml

    $ ansible-playbook -i inventory --ask-become-pass main.yml

    $ cd ~/dotfiles
    $ bin/install
    $ bin/setup_osx
