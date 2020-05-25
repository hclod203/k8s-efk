sudo snap install helm --classic

helm repo add stable https://kubernetes-charts.storage.googleapis.com/

helm install elasticsearch stable/elasticsearch wait for few minutes..

kubectl apply -f .\fluentd-daemonset-elasticsearch.yaml

helm install kibana stable/kibana -f kibana-values.yaml

kubectl apply -f .\counter.yaml

Open Kibana dashboard.
