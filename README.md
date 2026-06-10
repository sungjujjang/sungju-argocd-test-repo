# Argo webhook test

This repo contains Kubernetes manifests for a simple Argo Events + Argo Workflows webhook forwarding test.

Apply the manifests with Argo CD, then:

```powershell
curl.exe -X POST http://10.0.0.200:30081/webhook -H "Content-Type: application/json" -d "{\"hello\":\"argo\"}"
```

Open the receiver UI:

```text
http://10.0.0.200:30080/
```
