# Keycloak

To reproduce https://github.com/codecentric/helm-charts/issues/504
````
$ helm repo add codecentric https://codecentric.github.io/helm-charts
$ helm pull codecentric/keycloak --version 15.1.0
$ tar xfvz keycloak-15.1.0.tgz
$ helm lint ./keycloak/ --values ./val.yaml
````

Note:
````
$ uname -a
Darwin MacBook-Pro-de-Herve.local 20.6.0 Darwin Kernel Version 20.6.0
$ helm version
version.BuildInfo{Version:"v3.7.1", GitCommit:"1d11fcb5d3f3bf00dbe6fe31b8412839a96b3dc4", GitTreeState:"clean", GoVersion:"go1.17.2"}
````
