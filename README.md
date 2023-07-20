# Reverse Proxy Ansible role [![Ansible Lint](https://github.com/namelivia/ansible-reverse-proxy/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/namelivia/ansible-reverse-proxy/actions/workflows/ansible-lint.yml)

The project depends on the collection `community.docker` but apparently this [cannot be listed as a dependency](https://github.com/ansible/ansible/issues/62847) so make sure you add it to your `requirements.yml` file like:

```yml
---

collections:
  - community.docker

roles:
  - src: https://github.com/namelivia/ansible-reverse-proxy
```

## Required variables

 - `loki_url` Loki endpoint to send logs.
