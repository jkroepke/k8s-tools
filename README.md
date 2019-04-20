# k8s-tools
Tool and guides around the kubernetes / cloud native universe.

Its not a wall of bullshit just cerry picking good project with the taste of my opinion. 

# Contents

* ARA (Application Release Automation) 
* Monitoring
* Backup
* Certificates

# Problems & Solutions

# Big players

* Service Mesh
* Virtualization 
* Databases

## Monitoring

### Prometheus
https://prometheus.io/

Prometheus is the way to go. It's a replacement for the old nagios environment. You can also use prometheus for non cloud native applications and virtual machines.

### kube-state-metrics
https://github.com/kubernetes/kube-state-metrics

kube-state-metrics is a nice addon for your kubernetes cluster. With kube-state-metrics you can gain additional metrics from all your 1st party kubernetes objects.

You can find a wall of prometheus exporters here: https://github.com/prometheus/prometheus/wiki/Default-port-allocations

## Backup
https://github.com/heptio/velero

Velero (formerly Heptio Ark) gives you tools to back up and restore your Kubernetes cluster resources and persistent volumes.

## Certificates

### cert-manager
https://github.com/jetstack/cert-manager

If you want to use Istio but you (or your sec team) still wants full encryption inside your cluster, cert-manager can help u fine. You can also use cert-manager to gain Let's Encrypt certificates.



# Tools for Quick moments
https://github.com/weaveworks/footloose

footloose creates containers that look like virtual machines. Those containers run systemd as PID 1 and a ssh daemon that can be used to login into the container. Such "machines" behave very much like a VM, it's even possible to run dockerd in them :)

