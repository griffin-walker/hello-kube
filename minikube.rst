### Getting Started

Checkout minikube - Basic controls `here <https://minikube.sigs.k8s.io/docs/handbook/controls/>`_


Start a local cluster
 
.. code-block: bash

    minikube start
    😄  minikube v1.17.1 on Darwin 10.15.7
    ✨  Automatically selected the docker driver. Other choices: hyperkit, ssh
    👍  Starting control plane node minikube in cluster minikube
    🚜  Pulling base image ...
    💾  Downloading Kubernetes v1.20.2 preload ...
        > preloaded-images-k8s-v8-v1....: 133.01 MiB / 491.22 MiB  27.08% 403.05 Ki
        > preloaded-images-k8s-v8-v1....: 491.22 MiB / 491.22 MiB  100.00% 954.39 K
    🔥  Creating docker container (CPUs=2, Memory=1987MB) ...
    🐳  Preparing Kubernetes v1.20.2 on Docker 20.10.2 ...
        ▪ Generating certificates and keys ...
        ▪ Booting up control plane ...
        ▪ Configuring RBAC rules ...
    🔎  Verifying Kubernetes components...
    🌟  Enabled addons: storage-provisioner, default-storageclass
    🏄  Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default

.. code-block:bash

    minikube dashboard
    🔌  Enabling dashboard ...
    🤔  Verifying dashboard health ...
    🚀  Launching proxy ...
    🤔  Verifying proxy health ...
    🎉  Opening http://127.0.0.1:54862/api/v1/namespaces/kubernetes-dashboard/services/http:kubernetes-dashboard:/proxy/ in your default browser...

.. code-block: bash

    minikube stop # stop local cluster
    minikube delete # delete local cluster
    minikube delete --all # delete all local clusters and "profiles"

Profiles are 

> Kubernetes profiles enable cluster administrators and cluster managers to customize Kubernetes component settings for any clusters that they provision.

> A scheduling Profile allows you to configure the different stages of scheduling in the kube-scheduler. Each stage is exposed in an extension point. Plugins provide scheduling behaviors by implementing one or more of these extension points.