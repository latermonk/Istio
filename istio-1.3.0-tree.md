
```
.
├── bin
│   └── istioctl
├── install
│   ├── consul
│   │   ├── consul_config
│   │   │   ├── agent.json
│   │   │   ├── agent-loglevel.json
│   │   │   ├── disable_update_check.json
│   │   │   └── server.json
│   │   ├── istio.yaml
│   │   ├── kubeconfig
│   │   └── README.md
│   ├── gcp
│   │   ├── bootstrap
│   │   │   └── gcp_envoy_bootstrap.json
│   │   └── README.md
│   ├── kubernetes
│   │   ├── global-default-sidecar-scope.yaml
│   │   ├── helm
│   │   │   ├── helm-service-account.yaml
│   │   │   ├── istio
│   │   │   │   ├── charts
│   │   │   │   │   ├── certmanager
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── issuer.yaml
│   │   │   │   │   │   │   ├── NOTES.txt
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── rbac.yaml
│   │   │   │   │   │   │   └── serviceaccount.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── galley
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── validatingwebhookconfiguration.yaml.tpl
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── gateways
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── autoscale.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── preconfigured.yaml
│   │   │   │   │   │   │   ├── rolebindings.yaml
│   │   │   │   │   │   │   ├── role.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   └── service.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── grafana
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── dashboards
│   │   │   │   │   │   │   ├── citadel-dashboard.json
│   │   │   │   │   │   │   ├── galley-dashboard.json
│   │   │   │   │   │   │   ├── istio-mesh-dashboard.json
│   │   │   │   │   │   │   ├── istio-performance-dashboard.json
│   │   │   │   │   │   │   ├── istio-service-dashboard.json
│   │   │   │   │   │   │   ├── istio-workload-dashboard.json
│   │   │   │   │   │   │   ├── mixer-dashboard.json
│   │   │   │   │   │   │   └── pilot-dashboard.json
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── configmap-custom-resources.yaml
│   │   │   │   │   │   │   ├── configmap-dashboards.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── create-custom-resources-job.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── grafana-ports-mtls.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── ingress.yaml
│   │   │   │   │   │   │   ├── pvc.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── tests
│   │   │   │   │   │   │       └── test-grafana-connection.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── istiocoredns
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   └── service.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── kiali
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── demosecret.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── ingress.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── tests
│   │   │   │   │   │   │       └── test-kiali-connection.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── mixer
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── autoscale.yaml
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── config.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   └── service.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── nodeagent
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── daemonset.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   └── serviceaccount.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── pilot
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── autoscale.yaml
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── meshexpansion.yaml
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   └── service.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── prometheus
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── clusterrolebindings.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── ingress.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── tests
│   │   │   │   │   │   │       └── test-prometheus-connection.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── security
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── cleanup-secrets.yaml
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── create-custom-resources-job.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── enable-mesh-mtls.yaml
│   │   │   │   │   │   │   ├── enable-mesh-permissive.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── meshexpansion.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── tests
│   │   │   │   │   │   │       └── test-citadel-connection.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── sidecarInjectorWebhook
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── mutatingwebhook.yaml
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   └── service.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   └── tracing
│   │   │   │   │       ├── Chart.yaml
│   │   │   │   │       ├── templates
│   │   │   │   │       │   ├── deployment-jaeger.yaml
│   │   │   │   │       │   ├── deployment-zipkin.yaml
│   │   │   │   │       │   ├── _helpers.tpl
│   │   │   │   │       │   ├── ingress.yaml
│   │   │   │   │       │   ├── pvc.yaml
│   │   │   │   │       │   ├── service-jaeger.yaml
│   │   │   │   │       │   ├── service.yaml
│   │   │   │   │       │   └── tests
│   │   │   │   │       │       └── test-tracing-connection.yaml
│   │   │   │   │       └── values.yaml
│   │   │   │   ├── Chart.yaml
│   │   │   │   ├── example-values
│   │   │   │   │   ├── README.md
│   │   │   │   │   ├── values-istio-example-sds-vault.yaml
│   │   │   │   │   ├── values-istio-gateways.yaml
│   │   │   │   │   ├── values-istio-googleca.yaml
│   │   │   │   │   ├── values-istio-meshexpansion-gateways.yaml
│   │   │   │   │   └── values-istio-multicluster-gateways.yaml
│   │   │   │   ├── files
│   │   │   │   │   └── injection-template.yaml
│   │   │   │   ├── README.md
│   │   │   │   ├── requirements.yaml
│   │   │   │   ├── templates
│   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   ├── endpoints.yaml
│   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   ├── install-custom-resources.sh.tpl
│   │   │   │   │   ├── NOTES.txt
│   │   │   │   │   ├── _podDisruptionBudget.tpl
│   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   ├── service.yaml
│   │   │   │   │   └── sidecar-injector-configmap.yaml
│   │   │   │   ├── values-istio-demo-auth.yaml
│   │   │   │   ├── values-istio-demo.yaml
│   │   │   │   ├── values-istio-minimal.yaml
│   │   │   │   ├── values-istio-remote.yaml
│   │   │   │   ├── values-istio-sds-auth-control-plane-auth-disabled.yaml
│   │   │   │   ├── values-istio-sds-auth.yaml
│   │   │   │   └── values.yaml
│   │   │   ├── istio-cni
│   │   │   │   ├── Chart.yaml
│   │   │   │   ├── templates
│   │   │   │   │   ├── istio-cni.yaml
│   │   │   │   │   └── _labels.tpl
│   │   │   │   ├── values_gke.yaml
│   │   │   │   └── values.yaml
│   │   │   ├── istio-init
│   │   │   │   ├── Chart.yaml
│   │   │   │   ├── files
│   │   │   │   │   ├── crd-10.yaml
│   │   │   │   │   ├── crd-11.yaml
│   │   │   │   │   ├── crd-12.yaml
│   │   │   │   │   ├── crd-certmanager-10.yaml
│   │   │   │   │   └── crd-certmanager-11.yaml
│   │   │   │   ├── README.md
│   │   │   │   ├── templates
│   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   ├── configmap-crd-10.yaml
│   │   │   │   │   ├── configmap-crd-11.yaml
│   │   │   │   │   ├── configmap-crd-12.yaml
│   │   │   │   │   ├── configmap-crd-certmanager-10.yaml
│   │   │   │   │   ├── configmap-crd-certmanager-11.yaml
│   │   │   │   │   ├── job-crd-10.yaml
│   │   │   │   │   ├── job-crd-11.yaml
│   │   │   │   │   ├── job-crd-12.yaml
│   │   │   │   │   ├── job-crd-certmanager-10.yaml
│   │   │   │   │   ├── job-crd-certmanager-11.yaml
│   │   │   │   │   └── serviceaccount.yaml
│   │   │   │   └── values.yaml
│   │   │   └── README.md
│   │   ├── istio-demo-auth.yaml
│   │   ├── istio-demo.yaml
│   │   ├── mesh-expansion.yaml
│   │   ├── namespace.yaml
│   │   ├── operator
│   │   │   ├── charts
│   │   │   │   ├── crds
│   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   ├── files
│   │   │   │   │   │   ├── crd-10.yaml
│   │   │   │   │   │   ├── crd-11.yaml
│   │   │   │   │   │   ├── crd-12.yaml
│   │   │   │   │   │   ├── crd-certmanager-10.yaml
│   │   │   │   │   │   └── crd-certmanager-11.yaml
│   │   │   │   │   ├── kustomization.yaml
│   │   │   │   │   └── templates
│   │   │   │   │       ├── crds.yaml
│   │   │   │   │       └── namespaces.yaml
│   │   │   │   ├── gateways
│   │   │   │   │   ├── istio-egress
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── NOTES.txt
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── autoscale.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── preconfigured.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   └── service.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   └── istio-ingress
│   │   │   │   │       ├── Chart.yaml
│   │   │   │   │       ├── NOTES.txt
│   │   │   │   │       ├── templates
│   │   │   │   │       │   ├── addongateway.yaml
│   │   │   │   │       │   ├── _affinity.tpl
│   │   │   │   │       │   ├── autoscale.yaml
│   │   │   │   │       │   ├── certificate.yaml
│   │   │   │   │       │   ├── deployment.yaml
│   │   │   │   │       │   ├── gateway.yaml
│   │   │   │   │       │   ├── hosts.yaml
│   │   │   │   │       │   ├── meshexpansion.yaml
│   │   │   │   │       │   ├── poddisruptionbudget.yaml
│   │   │   │   │       │   ├── preconfigured.yaml
│   │   │   │   │       │   ├── rolebindings.yaml
│   │   │   │   │       │   ├── role.yaml
│   │   │   │   │       │   ├── serviceaccount.yaml
│   │   │   │   │       │   ├── service.yaml
│   │   │   │   │       │   └── sidecar.yaml
│   │   │   │   │       └── values.yaml
│   │   │   │   ├── istio-cni
│   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   ├── templates
│   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   ├── configmap-cni.yaml
│   │   │   │   │   │   ├── daemonset.yaml
│   │   │   │   │   │   └── serviceaccount.yaml
│   │   │   │   │   ├── values_gke.yaml
│   │   │   │   │   └── values.yaml
│   │   │   │   ├── istio-control
│   │   │   │   │   ├── istio-autoinject
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── files
│   │   │   │   │   │   │   └── injection-template.yaml
│   │   │   │   │   │   ├── NOTES.txt
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── mutatingwebhook.yaml
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── sidecar-injector-configmap.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── istio-config
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── OWNERS
│   │   │   │   │   │   ├── README.md
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap-envoy.yaml
│   │   │   │   │   │   │   ├── configmap-mesh.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── validatingwebhookconfiguration.yaml.tpl
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   └── istio-discovery
│   │   │   │   │       ├── Chart.yaml
│   │   │   │   │       ├── NOTES.txt
│   │   │   │   │       ├── templates
│   │   │   │   │       │   ├── _affinity.tpl
│   │   │   │   │       │   ├── autoscale.yaml
│   │   │   │   │       │   ├── clusterrolebinding.yaml
│   │   │   │   │       │   ├── clusterrole.yaml
│   │   │   │   │       │   ├── configmap-envoy.yaml
│   │   │   │   │       │   ├── configmap.yaml
│   │   │   │   │       │   ├── deployment.yaml
│   │   │   │   │       │   ├── enable-mesh-mtls.yaml
│   │   │   │   │       │   ├── _helpers.tpl
│   │   │   │   │       │   ├── poddisruptionbudget.yaml
│   │   │   │   │       │   ├── serviceaccount.yaml
│   │   │   │   │       │   └── service.yaml
│   │   │   │   │       └── values.yaml
│   │   │   │   ├── istiocoredns
│   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   ├── templates
│   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   └── service.yaml
│   │   │   │   │   └── values.yaml
│   │   │   │   ├── istio-policy
│   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   ├── templates
│   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   ├── autoscale.yaml
│   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   ├── config.yaml
│   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   ├── _helpers.tpl
│   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   └── service.yaml
│   │   │   │   │   └── values.yaml
│   │   │   │   ├── istio-telemetry
│   │   │   │   │   ├── grafana
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── dashboards
│   │   │   │   │   │   │   ├── galley-dashboard.json
│   │   │   │   │   │   │   ├── istio-mesh-dashboard.json
│   │   │   │   │   │   │   ├── istio-performance-dashboard.json
│   │   │   │   │   │   │   ├── istio-service-dashboard.json
│   │   │   │   │   │   │   ├── istio-workload-dashboard.json
│   │   │   │   │   │   │   ├── mixer-dashboard.json
│   │   │   │   │   │   │   └── pilot-dashboard.json
│   │   │   │   │   │   ├── fix_datasources.sh
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── configmap-dashboards.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── destination-rule.yaml
│   │   │   │   │   │   │   ├── grafana-policy.yaml
│   │   │   │   │   │   │   ├── pvc.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── tests
│   │   │   │   │   │   │       └── test-grafana-connection.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── kiali
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── demosecret.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   └── service.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── mixer-telemetry
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── autoscale.yaml
│   │   │   │   │   │   │   ├── clusterrolebinding.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap-envoy.yaml
│   │   │   │   │   │   │   ├── config.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── poddisruptionbudget.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── stackdriver.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── prometheus
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── clusterrolebindings.yaml
│   │   │   │   │   │   │   ├── clusterrole.yaml
│   │   │   │   │   │   │   ├── configmap.yaml
│   │   │   │   │   │   │   ├── deployment.yaml
│   │   │   │   │   │   │   ├── destination-rule.yaml
│   │   │   │   │   │   │   ├── inrgess.yaml
│   │   │   │   │   │   │   ├── serviceaccount.yaml
│   │   │   │   │   │   │   ├── service.yaml
│   │   │   │   │   │   │   └── tests
│   │   │   │   │   │   │       └── test-prometheus-connection.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   ├── prometheus-operator
│   │   │   │   │   │   ├── Chart.yaml
│   │   │   │   │   │   ├── templates
│   │   │   │   │   │   │   ├── _affinity.tpl
│   │   │   │   │   │   │   ├── prometheus.yaml
│   │   │   │   │   │   │   └── servicemonitors.yaml
│   │   │   │   │   │   └── values.yaml
│   │   │   │   │   └── tracing
│   │   │   │   │       ├── Chart.yaml
│   │   │   │   │       ├── templates
│   │   │   │   │       │   ├── _affinity.tpl
│   │   │   │   │       │   ├── deployment-jaeger.yaml
│   │   │   │   │       │   ├── deployment-opencensus.yaml
│   │   │   │   │       │   ├── deployment-zipkin.yaml
│   │   │   │   │       │   ├── pvc.yaml
│   │   │   │   │       │   ├── service-jaeger.yaml
│   │   │   │   │       │   └── service.yaml
│   │   │   │   │       └── values.yaml
│   │   │   │   └── security
│   │   │   │       ├── certmanager
│   │   │   │       │   ├── Chart.yaml
│   │   │   │       │   ├── templates
│   │   │   │       │   │   ├── _affinity.tpl
│   │   │   │       │   │   ├── deployment.yaml
│   │   │   │       │   │   ├── issuer.yaml
│   │   │   │       │   │   ├── NOTES.txt
│   │   │   │       │   │   ├── poddisruptionbudget.yaml
│   │   │   │       │   │   ├── rbac.yaml
│   │   │   │       │   │   └── serviceaccount.yaml
│   │   │   │       │   └── values.yaml
│   │   │   │       ├── citadel
│   │   │   │       │   ├── Chart.yaml
│   │   │   │       │   ├── templates
│   │   │   │       │   │   ├── _affinity.tpl
│   │   │   │       │   │   ├── clusterrolebinding.yaml
│   │   │   │       │   │   ├── clusterrole.yaml
│   │   │   │       │   │   ├── deployment.yaml
│   │   │   │       │   │   ├── _helpers.tpl
│   │   │   │       │   │   ├── NOTES.txt
│   │   │   │       │   │   ├── poddisruptionbudget.yaml
│   │   │   │       │   │   ├── serviceaccount.yaml
│   │   │   │       │   │   └── service.yaml
│   │   │   │       │   └── values.yaml
│   │   │   │       └── nodeagent
│   │   │   │           ├── Chart.yaml
│   │   │   │           ├── templates
│   │   │   │           │   ├── _affinity.tpl
│   │   │   │           │   ├── clusterrolebinding.yaml
│   │   │   │           │   ├── clusterrole.yaml
│   │   │   │           │   ├── daemonset.yaml
│   │   │   │           │   └── serviceaccount.yaml
│   │   │   │           └── values.yaml
│   │   │   ├── profiles
│   │   │   │   ├── default.yaml
│   │   │   │   ├── demo-auth.yaml
│   │   │   │   ├── demo.yaml
│   │   │   │   ├── minimal.yaml
│   │   │   │   └── sds.yaml
│   │   │   ├── versions.yaml
│   │   │   └── version.yaml
│   │   └── README.md
│   ├── README.md
│   └── tools
│       ├── setupIstioVM.sh
│       └── setupMeshEx.sh
├── istio.VERSION
├── LICENSE
├── README.md
├── samples
│   ├── bookinfo
│   │   ├── networking
│   │   │   ├── bookinfo-gateway.yaml
│   │   │   ├── certmanager-gateway.yaml
│   │   │   ├── destination-rule-all-mtls.yaml
│   │   │   ├── destination-rule-all.yaml
│   │   │   ├── destination-rule-reviews.yaml
│   │   │   ├── egress-rule-google-apis.yaml
│   │   │   ├── fault-injection-details-v1.yaml
│   │   │   ├── ROUTING_RULE_MIGRATION.md
│   │   │   ├── virtual-service-all-v1.yaml
│   │   │   ├── virtual-service-details-v2.yaml
│   │   │   ├── virtual-service-ratings-db.yaml
│   │   │   ├── virtual-service-ratings-mysql-vm.yaml
│   │   │   ├── virtual-service-ratings-mysql.yaml
│   │   │   ├── virtual-service-ratings-test-abort.yaml
│   │   │   ├── virtual-service-ratings-test-delay.yaml
│   │   │   ├── virtual-service-reviews-50-v3.yaml
│   │   │   ├── virtual-service-reviews-80-20.yaml
│   │   │   ├── virtual-service-reviews-90-10.yaml
│   │   │   ├── virtual-service-reviews-jason-v2-v3.yaml
│   │   │   ├── virtual-service-reviews-test-v2.yaml
│   │   │   ├── virtual-service-reviews-v2-v3.yaml
│   │   │   └── virtual-service-reviews-v3.yaml
│   │   ├── platform
│   │   │   ├── consul
│   │   │   │   ├── bookinfo.sidecars.yaml
│   │   │   │   ├── bookinfo.yaml
│   │   │   │   ├── cleanup.sh
│   │   │   │   ├── destination-rule-all.yaml
│   │   │   │   ├── README.md
│   │   │   │   ├── virtual-service-all-v1.yaml
│   │   │   │   ├── virtual-service-ratings-test-abort.yaml
│   │   │   │   ├── virtual-service-ratings-test-delay.yaml
│   │   │   │   ├── virtual-service-reviews-50-v3.yaml
│   │   │   │   ├── virtual-service-reviews-test-v2.yaml
│   │   │   │   ├── virtual-service-reviews-v2-v3.yaml
│   │   │   │   └── virtual-service-reviews-v3.yaml
│   │   │   └── kube
│   │   │       ├── bookinfo-certificate.yaml
│   │   │       ├── bookinfo-db.yaml
│   │   │       ├── bookinfo-details-v2.yaml
│   │   │       ├── bookinfo-details.yaml
│   │   │       ├── bookinfo-ingress.yaml
│   │   │       ├── bookinfo-mysql.yaml
│   │   │       ├── bookinfo-ratings-discovery.yaml
│   │   │       ├── bookinfo-ratings-v2-mysql-vm.yaml
│   │   │       ├── bookinfo-ratings-v2-mysql.yaml
│   │   │       ├── bookinfo-ratings-v2.yaml
│   │   │       ├── bookinfo-ratings.yaml
│   │   │       ├── bookinfo-reviews-v2.yaml
│   │   │       ├── bookinfo.yaml
│   │   │       ├── cleanup.sh
│   │   │       ├── productpage-nodeport.yaml
│   │   │       ├── rbac
│   │   │       │   ├── details-reviews-policy-permissive.yaml
│   │   │       │   ├── details-reviews-policy.yaml
│   │   │       │   ├── mongodb-policy.yaml
│   │   │       │   ├── namespace-policy.yaml
│   │   │       │   ├── productpage-policy.yaml
│   │   │       │   ├── ratings-policy.yaml
│   │   │       │   ├── rbac-config-on-mongodb.yaml
│   │   │       │   ├── rbac-config-on-permissive.yaml
│   │   │       │   ├── rbac-config-ON.yaml
│   │   │       │   └── rbac-permissive-telemetry.yaml
│   │   │       └── README.md
│   │   ├── policy
│   │   │   ├── mixer-rule-deny-ip-crd.yaml
│   │   │   ├── mixer-rule-deny-ip.yaml
│   │   │   ├── mixer-rule-deny-label-crd.yaml
│   │   │   ├── mixer-rule-deny-label.yaml
│   │   │   ├── mixer-rule-deny-serviceaccount.yaml
│   │   │   ├── mixer-rule-deny-whitelist-crd.yaml
│   │   │   ├── mixer-rule-deny-whitelist.yaml
│   │   │   ├── mixer-rule-ingress-denial.yaml
│   │   │   ├── mixer-rule-kubernetesenv-telemetry.yaml
│   │   │   ├── mixer-rule-productpage-ratelimit-crd.yaml
│   │   │   ├── mixer-rule-productpage-ratelimit.yaml
│   │   │   ├── mixer-rule-productpage-redis-quota-fixed-window.yaml
│   │   │   ├── mixer-rule-productpage-redis-quota-rolling-window.yaml
│   │   │   ├── mixer-rule-ratings-denial.yaml
│   │   │   ├── mixer-rule-ratings-ratelimit.yaml
│   │   │   ├── mixer-rule-ratings-redis-quota-fixed-window.yaml
│   │   │   ├── mixer-rule-ratings-redis-quota-rolling-window.yaml
│   │   │   ├── prometheus-adapter-deployment.yaml
│   │   │   └── prometheus-oop-rule.yaml
│   │   ├── README.md
│   │   ├── src
│   │   │   ├── mongodb
│   │   │   │   └── ratings_data.json
│   │   │   ├── productpage
│   │   │   │   ├── requirements.txt
│   │   │   │   └── test-requirements.txt
│   │   │   └── ratings
│   │   │       └── package.json
│   │   ├── swagger.yaml
│   │   └── telemetry
│   │       ├── fluentd-istio-crd.yaml
│   │       ├── fluentd-istio.yaml
│   │       ├── log-entry-crd.yaml
│   │       ├── log-entry.yaml
│   │       ├── metrics-crd.yaml
│   │       ├── metrics.yaml
│   │       ├── tcp-metrics-crd.yaml
│   │       └── tcp-metrics.yaml
│   ├── certs
│   │   ├── ca-cert.pem
│   │   ├── ca-key.pem
│   │   ├── cert-chain.pem
│   │   ├── README.md
│   │   └── root-cert.pem
│   ├── custom-bootstrap
│   │   ├── custom-bootstrap.yaml
│   │   ├── example-app.yaml
│   │   └── README.md
│   ├── external
│   │   ├── aptget.yaml
│   │   ├── github.yaml
│   │   ├── pypi.yaml
│   │   └── README.md
│   ├── fortio
│   │   └── stackdriver.yaml
│   ├── health-check
│   │   ├── liveness-command.yaml
│   │   ├── liveness-http-same-port.yaml
│   │   └── liveness-http.yaml
│   ├── helloworld
│   │   ├── helloworld-gateway.yaml
│   │   ├── helloworld.yaml
│   │   ├── README.md
│   │   └── src
│   │       └── requirements.txt
│   ├── httpbin
│   │   ├── httpbin-gateway.yaml
│   │   ├── httpbin-nodeport.yaml
│   │   ├── httpbin-vault.yaml
│   │   ├── httpbin.yaml
│   │   ├── policy
│   │   │   ├── keyval-template.yaml
│   │   │   └── keyval.yaml
│   │   ├── README.md
│   │   └── sample-client
│   │       └── fortio-deploy.yaml
│   ├── https
│   │   ├── default.conf
│   │   └── nginx-app.yaml
│   ├── kubernetes-blog
│   │   ├── bookinfo-ratings.yaml
│   │   ├── bookinfo-reviews-v2.yaml
│   │   └── bookinfo-v1.yaml
│   ├── rawvm
│   │   └── README.md
│   ├── README.md
│   ├── sleep
│   │   ├── policy
│   │   │   ├── sni-serviceaccount.yaml
│   │   │   └── sni-wikipedia.yaml
│   │   ├── README.md
│   │   ├── sleep-vault.yaml
│   │   ├── sleep.yaml
│   │   └── telemetry
│   │       └── sni-logging.yaml
│   ├── tcp-echo
│   │   ├── README.md
│   │   ├── tcp-echo-20-v2.yaml
│   │   ├── tcp-echo-all-v1.yaml
│   │   ├── tcp-echo-services.yaml
│   │   └── tcp-echo.yaml
│   └── websockets
│       ├── app.yaml
│       ├── README.md
│       └── route.yaml
├── tools
│   ├── cache_buster.yaml
│   ├── checker
│   │   ├── checker.go
│   │   ├── envvarlinter
│   │   │   ├── envvar_test.go
│   │   │   ├── main.go
│   │   │   ├── README.md
│   │   │   ├── rules
│   │   │   │   ├── no_os_env.go
│   │   │   │   └── util.go
│   │   │   ├── rules_matcher.go
│   │   │   ├── testdata
│   │   │   │   └── envuse.go
│   │   │   └── whitelist.go
│   │   ├── README.md
│   │   ├── report.go
│   │   ├── rule.go
│   │   ├── testlinter
│   │   │   ├── e2etest_lint_test.go
│   │   │   ├── integtest_lint_test.go
│   │   │   ├── lint_rules_list.go
│   │   │   ├── main.go
│   │   │   ├── README.md
│   │   │   ├── rules
│   │   │   │   ├── no_goroutine.go
│   │   │   │   ├── no_short.go
│   │   │   │   ├── no_sleep.go
│   │   │   │   ├── short_skip.go
│   │   │   │   ├── skip_issue.go
│   │   │   │   └── util.go
│   │   │   ├── rules_matcher.go
│   │   │   ├── testdata
│   │   │   │   ├── e2e
│   │   │   │   │   └── e2e_test.go
│   │   │   │   ├── integration
│   │   │   │   │   └── integtest_test.go
│   │   │   │   ├── integtest_integ_test.go
│   │   │   │   └── unit_test.go
│   │   │   ├── testlinter
│   │   │   ├── unittest_lint_test.go
│   │   │   └── whitelist.go
│   │   └── whitelist.go
│   ├── convert_perf_results.py
│   ├── convert_RbacConfig_to_ClusterRbacConfig.sh
│   ├── docker-dev
│   │   ├── Dockerfile
│   │   └── README.md
│   ├── dump_kubernetes.sh
│   ├── githubContrib
│   │   └── Contributions.txt
│   ├── hyperistio
│   │   ├── hyperistio.go
│   │   ├── hyperistio_test.go
│   │   ├── index.html
│   │   └── README.md
│   ├── _istioctl
│   ├── istioctl.bash
│   ├── istio-docker.mk
│   ├── istio-iptables
│   │   ├── main.go
│   │   └── pkg
│   │       └── dependencies
│   │           ├── implementation.go
│   │           ├── interface.go
│   │           └── stub.go
│   ├── license
│   │   ├── get_dep_licenses.go
│   │   ├── manual_append
│   │   │   ├── signalfx.txt
│   │   │   └── siphash.txt
│   │   └── README.md
│   ├── packaging
│   │   ├── common
│   │   │   ├── envoy_bootstrap_drain.json
│   │   │   ├── envoy_bootstrap_v2.json
│   │   │   ├── istio-auth-node-agent.service
│   │   │   ├── istio-ca.sh
│   │   │   ├── istio-iptables.sh
│   │   │   ├── istio-node-agent-start.sh
│   │   │   ├── istio.service
│   │   │   ├── istio-start.sh
│   │   │   └── sidecar.env
│   │   ├── deb
│   │   │   ├── deb_test.sh
│   │   │   ├── Dockerfile
│   │   │   ├── istio.mk
│   │   │   └── postinst.sh
│   │   ├── packaging.mk
│   │   └── rpm
│   │       ├── build-istio-rpm.sh
│   │       ├── build-proxy-rpm.sh
│   │       ├── Dockerfile.build
│   │       ├── istio
│   │       │   └── istio.spec
│   │       ├── proxy
│   │       │   ├── bazelrc
│   │       │   └── istio-proxy.spec
│   │       └── rpm.mk
│   ├── perf_istio_rules.yaml
│   ├── perf_k8svcs.yaml
│   ├── perf_setup.svg
│   ├── README.md
│   ├── rules.yml
│   ├── run_canonical_perf_tests.sh
│   ├── setup_perf_cluster.sh
│   ├── setup_run
│   ├── update_all
│   └── vagrant
│       ├── provision-vagrant.sh
│       └── Vagrantfile
└── tree.txt

155 directories, 672 files

```
