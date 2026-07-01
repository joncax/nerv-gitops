# nerv-gitops
Repositório central de configuração GitOps para o cluster nerv-server-k8s-01.
Este repositório é a única fonte lida pelo ArgoCD - contém os Helm charts e
os manifests de Application para todas as apps geridas.

## Estrutura

apps/
|--- nerv-dashboard/ <- Helm chart (Chart.yaml, values.yaml, templates/)
argocd/
|--- applications/ <- Manifests "Application" do ArgoCD

## Apps geridas

| App | Estado | Namespace(s) |
| --- | --- | --- |
| nerv-dashboard | Em migração | nerv-dashboard |

## Repositório de código associado

- https://github.com/joncax/nerv-dashboard
