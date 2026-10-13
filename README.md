# Upstream subchart example

This sample parent chart declares the Bitnami Redis chart as an upstream dependency.

## Commands

```powershell
helm dependency update .
helm lint .
helm template demo .
```

Set `redis.enabled=false` to disable the dependency when rendering:

```powershell
helm template demo . --set redis.enabled=false
```
