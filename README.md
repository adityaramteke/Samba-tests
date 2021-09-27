# Samba-tests
Repository contain declarative tests required for 
[Samba in kubernetes](https://github.com/samba-in-kubernetes).

## Prerequisites
You need to have a kubernetes cluster running. For example,
[minikube](https://kubernetes.io/docs/setup/learning-environment/minikube/)
is sufficient.

Install [KUbernetes Test TooL (KUTTL)](https://github.com/kudobuilder/kuttl)
binaries for linux from [release page](https://github.com/kudobuilder/kuttl/releases).

Make sure to configure the [Samba Operator](https://github.com/samba-in-kubernetes/samba-operator):
```
make deploy
```

## Run test
Let's run this test suite:
```
kubectl kuttl test ./kuttl-test/e2e
```

