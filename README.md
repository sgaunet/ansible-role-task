
This role is **obsolete**, please, [use this role instead.](https://github.com/sgaunet/ansible-role-gh-release-installer/blob/main/docs/available_tools.md#task)

# Ansible Role: task

[![CI](https://github.com/sgaunet/ansible-role-task/workflows/CI/badge.svg?event=push)](https://github.com/sgaunet/ansible-role-task/actions?query=workflow%3ACI)

An Ansible Role that installs [task](https://github.com/sgaunet/task) on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    task_version: "3.35.1"            # or "latest" (default)
    task_bin_path: "/usr/local/bin"
    task_tmp_directory: "{{ lookup('env', 'TMPDIR') | default('/tmp', true) }}"
    task_os: "linux"
    task_arch: "amd64"

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - sgaunet.task
```

## License

MIT
