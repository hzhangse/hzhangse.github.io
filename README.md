# hzhangse.github.io
<<<<<<< HEAD
helm lint spark-operator-chart 
helm package spark-operator-chart 
helm repo index --url https://hzhangse.github.io .
=======
helm lint spark-operator-chart <br/>
helm package spark-operator-chart <br/>
helm repo index --url https://hzhangse.github.io .  <br/>
>>>>>>> 51d18c5f2ed92c47f71dce4da0fe9c9a72ce41b2


helm repo remove spark-operator <br/>
helm repo add spark-operator https://hzhangse.github.io/ <br/>
##spark-on-k8s-operator 

helm install my-release spark-operator/spark-operator --namespace spark-operator --create-namespace <br/>
helm install my-release spark-operator/spark-operator --namespace spark-operator --set webhook.enable=true --set sparkJobNamespace=test-ns <br/>
helm uninstall my-release -n spark-operator <br/>
helm install my-release spark-operator/spark-operator --namespace spark-operator --set webhook.enable=true --set sparkJobNamespace=test-ns --dry-run --debug

