---
title: "oc"
draft: false
---

# oc

(OpenShift CLI)

## Download
curl -LO https://mirror.openshift.com/pub/openshift-v4/clients/ocp/stable-4.6/openshift-client-linux.tar.gz

## Extract
```bash
tar xfvz openshift-client-linux.tar.gz
```

## Install

Put the oc and kubectl binary into ~/bin


## Copy login command from OpenShift cluster
https://<cluster url>/k8s/cluster/projects

Click on the username in the top right corner and then select 'Copy login command'.

```bash
oc login --token=sha256~<token> --server=https://<webendpunkt>
```

This command will create a cinfiguration file for kubectl under `~/.kube/config`

Load configuration into variable

```bash
export KUBECONFIG=$HOME/.kube/config
```

Now the kubectl can be used.
