# local externalsecrets

Provides a patched version of the `ExternalSecrets` custom resource to work around [#476](https://github.com/godaddy/kubernetes-external-secrets/issues/476) so that we can support local secrets (no secrets storage back end, just local kubernetes Secret resources)

This chart is expected to be used by a [Jenkins X V3](https://jenkins-x.io/docs/v3/) installation if its using `secretStorage: local` in `jx-requirements.yml`

Here's an [example of its use](https://github.com/jx3-gitops-repositories/jx3-kubernetes/blob/main/helmfiles/jx/helmfile.yaml#L56-L60) when using a vanilla kubernetes cluster without using Vault or a cloud native secret store
