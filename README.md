# Helm + GitOps + ArgoCD Sample

這是一個示範專案，展示如何使用 Helm 搭配 GitOps 與 ArgoCD 自動部署 Nginx 應用。

## 架構說明

- `helm-chart/nginx/`：Helm chart，定義 Nginx 部署模板
- `apps/nginx/`：GitOps 配置，供 ArgoCD 同步
- `argocd-apps/nginx-helm-app.yaml`：ArgoCD 的 Application 配置，將 chart 安裝到 K8s 上
