# hzhangse.github.io
helm lint spark-operator-chart 
helm package spark-operator-chart
helm repo index --url https://hzhangse.github.io .


helm repo remove spark-operator
helm repo add spark-operator https://hzhangse.github.io/
##spark-on-k8s-operator

helm install my-release spark-operator/spark-operator --namespace spark-operator --create-namespace
helm install my-release spark-operator/spark-operator --namespace spark-operator --set webhook.enable=true --set sparkJobNamespace=test-ns
helm uninstall my-release -n spark-operator
