# renovate-issue-19517

## Current Behavior

Renonvate incorrectly extracts `newDepName`

```
DEBUG: depName mismatch (repository=onedr0p/home-ops, packageFile=kubernetes/flux/config/flux.yaml, branch=renovate/ghcr.io-fluxcd-flux-manifests-0.x)
       "manager": "flux",
       "currentDepName": "ghcr.io/fluxcd/flux-manifests",
       "newDepName": "ghcr.io/fluxcd/flux-manifests:"
 WARN: Error updating branch: update failure (repository=onedr0p/home-ops, branch=renovate/ghcr.io-fluxcd-flux-manifests-0.x)
```

## Expected Behavior

Renovate should open a PR to bump the tag in the OCIRepository Spec.
