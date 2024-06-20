# Ansible Role : deploy_histtimeformat

[![CI](https://github.com/glillico/ansible-role-deploy_histtimeformat/workflows/CI/badge.svg)](https://github.com/glillico/ansible-role-deploy_histtimeformat/actions?query=workflow%3ACI)

Copies a script into /etc/profile.d/ thart will be run at login buy the bash shell, and sets the HISTTIMEFORMAT environment variable.

When this is environment variable is set, the history command will show the date and time the command was run using the configured format which is this case is `DD/MM/YY HH:MM:SS`

### Environment variable set.

```
1355  18/06/24 09:07:10 ls
```

### Environment variable not set.

```
1355  ls
```

## Requirements

None.

## Role Variables

None.

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
         - glillico.deploy_histtimeformat

## License

MIT

## Author Information

Created in 2024 by Graham Lillico.
