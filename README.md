# ansible-ee
This repository contains a basic ansible execution environment.

## features
* uses latest version of ansible-core 2.12
* uses [mitogen](https://github.com/mitogen-hq/mitogen) per default

## usage

### pull ansible ee
```text
podman pull ghcr.io/linxside/ansible-ee:latest
```

### use ee in ansible-runner
```text
ansible-runner run --container-image ghcr.io/linxside/ansible-ee:latest -p <YOUR-PLAYBOOK>.yaml
```

### use ee in ansible-navigator
```text
ansible-navigator --eei ghcr.io/linxside/ansible-ee:latest
```