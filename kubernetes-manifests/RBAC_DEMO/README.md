# Service account token 

```powershell
$SecretName = kubectl -n rbac-demo get sa demo-user -o jsonpath="{.secrets[0].name}"
$Base64Token = kubectl -n rbac-demo get secret $SecretName -o jsonpath="{.data.token}"
$Token = kubectl -n rbac-demo create token demo-user
```

# Get API Server URL and CA Cert Path

```powershell
$APIServer = kubectl config view --minify -o jsonpath="{.clusters[0].cluster.server}"
```

CA cert location 

```powershell
$CACertPath = "$(minikube profile list --output json | ConvertFrom-Json).valid[0].Config.KubernetesConfig.CAFile"
```

If dowsnt work try manually

```powershell
curl.exe --header "Authorization: Bearer $Token" --cacert $CACertPath "$APIServer/api/v1/namespaces/rbac-demo/pods"
```

