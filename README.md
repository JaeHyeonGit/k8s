# Kubernetes Cluster Install
Kubeadm을 통해 설치 진행

container runtime : containerd, 
Container Network Interface : Calico


#20260403 각 NODE에 배포되어 있는 POD 통신 불가능 조치완료
InitIalize 하는 과정에서 pod network의 cidr을 지정해줘야 함

# Control Node의 InitIalize
sudo kubeadm init --pod-network-cidr=10.244.0.0/16


