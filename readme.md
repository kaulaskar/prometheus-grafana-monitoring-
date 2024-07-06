kubectl apply -f prometheus-config.yaml
kubectl apply -f prometheus-statefulset.yaml
kubectl apply -f grafana-deployment.yaml
kubectl apply -f node-exporter-daemonset.yaml


--

aws eks --region us-east-1 update-kubeconfig --name <cluste-name>