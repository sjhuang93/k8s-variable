# k8s-variable
Manage variables over namespace easily.

## How to use

example

```yaml
## Global variables
global:
  platform: on-premises
  environment: dev

variables:
  - name: test-config
    namespaces:
    - default
    secrets:
      k1: "v1"
      k2: "v2"
    configs:
      k3: "v3"
      k4: "v4"
```