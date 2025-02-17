[![Travis CI Build Status](https://api.travis-ci.com/AndriyKalashnykov/spring-microservices-k8s.svg?branch=master)](https://travis-ci.com/github/AndriyKalashnykov/spring-microservices-k8s)
[![GitHub CI Status](https://github.com/AndriyKalashnykov/spring-microservices-k8s/workflows/ci/badge.svg)](https://github.com/AndriyKalashnykov/spring-microservices-k8s/actions?query=workflow%3Aci)
### Java Microservices with Spring Boot and Spring Cloud Kubernetes
### https://tanzu.vmware.com/developer/guides/app-enhancements-spring-k8s/

### Pre-requisites

- OS: Mac or Linux
- [Docker](https://docs.docker.com/install/)
- [Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)
- [Virtualbox](https://www.virtualbox.org/manual/ch02.html)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [sdkman](https://sdkman.io/install)

    JDK 11.x
    
    ```shell
    sdk use java 11.0.10.hs-adpt
    ```
- [Apache Maven](https://maven.apache.org/install.html)
- [Curl](https://help.ubidots.com/en/articles/2165289-learn-how-to-install-run-curl-on-windows-macosx-linux)
- [HTTPie](https://httpie.org/doc#installation)
- [tree](http://mama.indstate.edu/users/ice/tree/)

### Clone repository

```bash
git clone git@github.com:AndriyKalashnykov/spring-microservices-k8s.git
```

### Start Kubernetes cluster

```bash
cd ./spring-microservices-k8s/scripts/
./start-cluster.sh
```

### Configure Kubernetes cluster

```bash
cd ./spring-microservices-k8s/scripts/
./setup-cluster.sh
```

### Deploy application to Kubernetes cluster

```bash
cd ./spring-microservices-k8s/scripts/
./install-all.sh
```

### Polulate test date

```bash
cd ./spring-microservices-k8s/scripts/
./populate-data.sh
```

### Observe Employee service logs

```bash
cd ./spring-microservices-k8s/scripts/
./employee-log.sh
```

### Open Swagger UI web interface

```bash
cd ./spring-microservices-k8s/scripts/
./gateway-open.sh
```

### Undeploy application from Kubernetes cluster

```bash
cd ./spring-microservices-k8s/scripts/
./delete-all.sh
```

### Delete Application specific Kubernetes cluster configuration (namespaces, clusterRole, etc.)

```bash
cd ./spring-microservices-k8s/scripts/
./destroy-cluster.sh
```

### Stop Kubernetes cluster

```bash
cd ./spring-microservices-k8s/scripts/
./stop-cluster.sh
```
