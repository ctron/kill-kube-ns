# kill-kube-ns

Kill a Kubernetes namespace/OpenShift project which is stuck in the state of "Terminating".

Also see: [kubernetes/kubernetes#60807](https://github.com/kubernetes/kubernetes/issues/60807)

This scripts automates the steps suggestes by some people on the comments of the issue.

**Note:** Use at your own risk! It works for me though.

## Usage

~~~sh
./kill-kube-ns myproject
~~~

**Note:** You will need to be logged in to your cluster, and have the necessary permissions. Make sure that your port `8001` is available.

## Pre-requisites

Your will need to have the following things installed:

* bash
* curl
* jq
* kubectl
