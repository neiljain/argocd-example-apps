# Ambassador using Helm Dependencies

This example application demonstrates how an OTS (off-the-shelf) helm chart can be retrieved and
pinned to a specific helm sem version from an upstream helm repository, and customized using a custom
values.yaml in the private git repository.

In this example, ambassador is pulled from the stable helm repo, and pinned to v6.3.1:

```yaml
dependencies:
- name: ambassador
  version: 6.3.1
  repository: https://getambassador.io
```

A custom values.yaml is used to customize the parameters
