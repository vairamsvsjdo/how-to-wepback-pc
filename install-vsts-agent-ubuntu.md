## Install Java
sudo apt update
sudo apt install default-jdk
java -version
sudo update-alternatives --config java
sudo nano /etc/environment
JAVA_HOME="/usr/lib/jvm/java-11-openjdk-amd64"
source /etc/environment
echo $JAVA_HOME

## Install Scala
https://www.scala-sbt.org/release/docs/Installing-sbt-on-Linux.html

echo "deb https://dl.bintray.com/sbt/debian /" | sudo tee -a /etc/apt/sources.list.d/sbt.list
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2EE0EA64E40A89B84B2DF73499E82A75642AC823
sudo apt-get update
sudo apt-get install sbt

## Install Docker
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
sudo apt update
apt-cache policy docker-ce
sudo apt install docker-ce
sudo usermod -aG docker ${USER}

## Relogin to get usermod effective
login username
sudo systemctl status docker
docker ps

## Install VSTS Azure DevOps Agent
https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/v2-linux?view=azure-devops

wget <download url>
~/$ mkdir myagent && cd myagent
~/myagent$ tar zxvf ~/vsts-agent-linux-x64-2.152.1.tar.gz
~/myagent$ ./config.sh
~/myagent$ ./run.sh

## start agent service
sudo ./svc.sh install
sudo ./svc.sh start
sudo ./svc.sh status
sudo ./svc.sh stop
