# Infrastructure Test project
This repository contains the Kubernetes config for a Nexus and a Jenkins master, both with persistent storage. Jenkins is pre-configured by the [](https://hub.docker.com/r/cwansart/jenkins-podman-slave) image to enable a special Jenkins agent image to connect automatically.

Nexus is not pre-configured yet. Add a hosted Docker registry with the http port `10080`.

## Start Jenkins+Agent+Nexus

```
$ kubectl apply -f config
```

## Delete

```
$ kubectl delete -f config
```