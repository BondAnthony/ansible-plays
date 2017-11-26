## Github SSH Keys
------------------

Quickly configure a remote system with your public keys.

### Required

Github account with ssh keys configured. Once your public key has been configured you should see the public key at the following endpoint: http://api.github.com/users/{{username}}/keys

Github API: 4.0

### How to Execute

Execute the play supplying the follow variables on the command line.

```yaml

user: ssh_user

github_user: github_handle

vms: remote_machines
```

Example Execution:

```
ansible-playbook github_ssh_keys.yml --extra-vars='{"vms":"cloud","github_user":"toilops","user":"root"}' --ask-pass --user root
```
