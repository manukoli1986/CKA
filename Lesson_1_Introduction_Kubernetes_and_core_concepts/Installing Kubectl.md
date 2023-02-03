# Installing and Configuring Kubectl for Linux

###  Documentation Link for kubectl

https://kubernetes.io/docs/tasks/tools/install-kubectl/   


### Here are the steps to install kubectl on a Linux system:

## Download the latest version of kubectl by running the following command in the terminal:
```bash
curl -LO https://dl.k8s.io/release/stable.txt
```

## Extract the version number from the above file and use it to download the corresponding kubectl binary:
```bash
KUBECTL_VERSION=$(cat stable.txt)
curl -LO https://dl.k8s.io/$KUBECTL_VERSION/bin/linux/amd64/kubectl
```

## Make the kubectl binary executable:
```bash
chmod +x kubectl
```

## Move the kubectl binary to a directory that is included in your PATH environment variable:
```bash
sudo mv kubectl /usr/local/bin/
```

## Verify the installation by running the following command:
```bash
kubectl version --client
```
## After following these steps, kubectl should be installed and ready to use on your Linux system.
