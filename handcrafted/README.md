# Grafana handcrafted dashboards

These dashboards have been hand crafted by the Bitnami SRE team.
All of them are ordered in subfolders depending the ambit of the dashboard.

Also, the `$datasource` variable has been configured in Grafana to allow multi-datasource setups.

All the dashboards that are present in this folder are meant to be migrated to _jsonnet_ in the near future.

The upgrade is done with the v1.22 cluster

<pre>
[root@k8s-master1 ~]# kubectl get nodes 
NAME          STATUS   ROLES                  AGE   VERSION
k8s-master1   Ready    control-plane,master   39m   v1.22.2
node1         Ready    <none>                 38m   v1.22.2
</pre>

**Kubernetes cluster capacity**
![Alt text](images/capacity.png?raw=true "Dashboard_1")

**Kubernetes resource usage per namespace and pod**
![Alt text](images/resource_per_pod_and_namespace.png?raw=true "Dashboard_2")
