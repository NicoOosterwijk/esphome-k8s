# ESPHome kustomization K8s

```
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  name: esphome
  namespace: fleet-default
  labels:
    esphome: enabled
spec:
  branch: main
  clientSecretName: auth-hp48c
  repo: https://github.com/NicoOosterwijk/esphome-k8s.git
  targets:
    - clusterGroup: esphome
```