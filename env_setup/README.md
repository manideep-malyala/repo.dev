# Tools Installation Guide for DevOps



#### VS CODE
[vs code](https://code.visualstudio.com/)

---

#### UPDATE YUM
`# yum update -y`


---
#### PYTHON 
`# yum install python -y`  <br>
`# python --version`

---

#### AWS CLI 
[reference](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

`# curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"`  
`# unzip awscliv2.zip`  
`# ./aws/install`  
`# aws --version`  


---

#### GIT 

`# yum install git -y`  
`# git version`   

---

#### JAVA

`# yum install java -y`  
`# java --version`   

---

#### APACHE MAVEN

[reference](https://maven.apache.org/)

`# cd /opt/`   
`# wget https://dlcdn.apache.org/maven/maven-3/3.9.6/binaries/apache-maven-3.9.6-bin.tar.gz`   
`# tar xzvf apache-maven-3.9.6-bin.tar.gz`   
`# vim /etc/profile.d/maven.sh`

> edit maven.sh file    
`export MAVEN_HOME=/opt/apache-maven-3.9.6`   
`export PATH=$PATH:$MAVEN_HOME/bin`

`# source /etc/profile`  
`# mvn -v` 

---

#### JENKINS

[reference](https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/)

`# cd /opt/`   
`# wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo`  
`# rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key`   
`# yum install jenkins -y`   
`# systemctl enable jenkins --now`   
`# systemctl status jenkins`   

---

#### DOCKER

`# yum install docker -y`   
`# usermod -aG docker jenkins`   
`# systemctl enable docker --now`   
`# systemctl status docker`

---

#### KUBECTL 

[reference](https://docs.aws.amazon.com/eks/latest/userguide/install-kubectl.html)

`# curl -O https://s3.us-west-2.amazonaws.com/amazon-eks/1.29.0/2024-01-04/bin/linux/amd64/kubectl`   
`# chmod +x ./kubectl`   
`# mkdir -p $HOME/bin && cp ./kubectl $HOME/bin/kubectl && export PATH=$HOME/bin:$PATH`    
`# echo 'export PATH=$HOME/bin:$PATH' >> ~/.bashrc`   
`# source ~/.bashrc`   
`# kubectl version --client`   

---

#### EKSCTL

[reference](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/setting-up-eksctl.html)

`# curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp`   
`# mv /tmp/eksctl /usr/local/bin`   
`# eksctl version`  

---

#### NODEJS

`# yum install nodejs -y`   
`# node -v`   
`# npm -v`   

---

#### MINIKUBE

[reference](https://minikube.sigs.k8s.io/docs/start/)   
`# curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64`   
`# install minikube-linux-amd64 /usr/local/bin/minikube`    
`# minikube start --driver docker`  

---

