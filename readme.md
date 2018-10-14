## Helpful Ansible Plays

I find my self from time to time repeating plays throughout different projects. I also sometimes forget, how did I solve this issue before. Ansible roles allow for you to build custom actions that can be imported into playbooks multiple times. While this process is extremely helpful, roles can be a little more than what one person needs. The other issue of course is you need access to Github, Galaxy or any SVN storing those roles.

This project is more of a catalog or learning repository for Ansible plays. Simple and to the point, providing new users of Ansible with some real world examples of how Ansible has made my automation life a lot easier!


### Getting Started

Ansible can be installed on a system using a number of different package managers or even running from source. I'll outline a couple options below.

1. Install Ansible on Red Hat system using `yum` or `dnf`
    ```
    $ yum install ansible
    ```
    ```
    $ dnf install ansible
    ```
2. Install Ansible using Python's `pip` package manager
    ```
    $ pip install ansible
    ```
    Of course if you don't have `pip` installed you need that installed first
    ```
    $ easy_install pip
    ```
3. Install Ansible on a Ubuntu system.
    ```
    $ apt-get install ansible
    ```
4. My favorite way of installing Ansible is directly from source. Now this option is a little more involved and requires more knownledge on the python development side but, you do have the ability to run the latest and great features and **bugs**. Word of advice if you do run from source please make sure you checkout a release tag when your hitting production systems.
    
    a. Clone the project directly from Github.
    ```
    $ git clone https://github.com/ansible/ansible.git --recursive
    $ cd ansible
    ```
    b. Source the `hacking/env-setup` script. Add the `-q` flag to run in quiet mode, reducing output to the screen.
    ```
    $ source ./hacking/env-setup
    ```
    