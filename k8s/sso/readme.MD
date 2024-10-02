Config API K8S
/etc/kubernetes/manifests/kube-apiserver.yaml

    - --oidc-client-id=kubernetes
    - --oidc-groups-claim=groups
    - --oidc-issuer-url=https://example.com
    - --oidc-username-claim=name

Create clusterrolebinding

kubectl create clusterrolebinding --clusterrole cluster-admin --group "authors" dex-admins

Open Browser 

https://dex-auth.example.com