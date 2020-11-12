# local-external-secrets

Provides a patched version of the `ExternalSecrets` custom resource to work around [#476](https://github.com/godaddy/kubernetes-external-secrets/issues/476) so that we can support local secrets (no secrets storage back end, just local kubernetes Secret resources)
