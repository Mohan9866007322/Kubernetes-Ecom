curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x kubectl
sudo mv kubectl /usr/local/bin/
kubectl version --client



curl --silent --location "https://github.com/eksctl-io/eksctl/releases/latest/download/eksctl_Linux_amd64.tar.gz" -o /tmp/eksctl.tar.gz
tar -xzf /tmp/eksctl.tar.gz -C /tmp
sudo mv /tmp/eksctl /usr/local/bin
