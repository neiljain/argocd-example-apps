# Kong using Helm Dependencies

This example application demonstrates how an OTS (off-the-shelf) helm chart can be retrieved and
pinned to a specific helm sem version from an upstream helm repository, and customized using a custom
values.yaml in the private git repository.

In this example, kong is pulled from the konghq helm repo, and pinned to v1.5.0:

```yaml
dependencies:
- name: kong
  version: 1.5.0
  repository: https://charts.konghq.com
```

A custom values.yaml is used to customize the parameters
