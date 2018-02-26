### Kubernetes Load Balancer Example
+ Greeting Service
+ Name Service

### Usage

```
minikube start
```

#### Build and push image
```
$ cd greeting-service
$ docker build -t nhatthai/greeting-service:latest .
$ docker push nhatthai/greeting-service:latest
```

#### Start Greeting Service
```
$ cd greeting-service
$ kubectl manifests/greeting-service
```

#### Build and push image
```
$ cd name-service
$ docker build -t nhatthai/name-service:latest .
$ docker push nhatthai/name-service:latest
```

#### Start Name Service
```
$ cd name-service
$ kubectl manifests/name-service
```

#### Run Greeting Service
http://192.168.99.100:31999/greeting


### Referrence
[Ribbon Example - GitHub](https://github.com/spring-cloud-incubator/spring-cloud-kubernetes/tree/master/spring-cloud-kubernetes-examples/kubernetes-circuitbreaker-ribbon-example)