# BuildSystemZero2One
1. [Vagrant](#vagrant)
2. [Oracle VM Virtualbox](#virtualbox)
3. [Centos(Vagrant+Oracle VM Virtualbox)](#centos)
4. [Docker](#docker)
5. [Nginx](#nginx)
6. [Openresty](#openresty)
7. [Redis](#redis)
8. [Mysql](#mysql)
9. [GitLab](#gitLab)
10. [Jenkins](#jenkins)
11. [Swagger](#swagger)
12. [SpringBoot](#springBoot)
13. [Redis+Lua](#redisLua)
14. [Jmeter](#jmeter)

<a id="vagrant"></a>
## Vagrant
1.Download url
https://www.vagrantup.com/downloads.html
![alt text](images/Vagrant/Vagrant1.PNG)

2.install</br>
<img src="images/Vagrant/Vagrant2.png" width="200"></br>
![alt text](images/Vagrant/Vagrant3.PNG)</br>
![alt text](images/Vagrant/Vagrant4.png)</br>
![alt text](images/Vagrant/Vagrant5.png)</br>
![alt text](images/Vagrant/Vagrant6.png)</br>
![alt text](images/Vagrant/Vagrant7.png)</br>
![alt text](images/Vagrant/Vagrant8.png)</br>
![alt text](images/Vagrant/Vagrant9.png)</br>
</br>
</br>
<a id="virtualbox"></a>
## Oracle VM Virtualbox
1.Download url
https://www.virtualbox.org/wiki/Downloads
![alt text](/images/Virtualbox/Virtualbox1.PNG?raw=true)

2.install</br>
<img src="images/Virtualbox/Virtualbox2.png" width="200"></br>
![alt text](images/Virtualbox/Virtualbox3.png)</br>
![alt text](images/Virtualbox/Virtualbox4.png)</br>
![alt text](images/Virtualbox/Virtualbox5.png)</br>
![alt text](images/Virtualbox/Virtualbox6.png)</br>
![alt text](images/Virtualbox/Virtualbox7.png)</br>
![alt text](images/Virtualbox/Virtualbox8.png)</br>
![alt text](images/Virtualbox/Virtualbox9.png)</br>
</br>
</br>

<a id="centos"></a>
## Centos(Vagrant+Oracle VM Virtualbox)
1.search and confirm centos version from vagrant repository</br>
vagrant repository url: https://app.vagrantup.com/boxes/search</br>
![alt text](images/Centos/centos1.png)</br>
![alt text](images/Centos/centos2.png)</br>

2.init centos </br>
command:
>vagrant init centos/7
![alt text](images/Centos/centos3.png)</br>
![alt text](images/Centos/centos4.png)</br>

3.open C:\Users\xxxx and confirm Vagrantfile</br>
![alt text](images/Centos/centos5.png)</br>

4.install vagrant-disksize plugin for specify the disk size</br>
command:vagrant plugin install vagrant-disksize</br>
![alt text](images/Centos/centos6.png)</br>
![alt text](images/Centos/centos7.png)</br>

5.edit Vagrantfile for specify the disk and memory size and ip</br>
add:</br>
  config.disksize.size = '300GB' </br>
  config.vm.provider "virtualbox" do |vb| </br>
     vb.memory = "2048"                   </br>
  end </br>
  config.vm.network "private_network", ip: "192.168.56.66"</br>
![alt text](images/Centos/centos8.png)</br>

6.auto download centos and start </br>
command:vagrant up</br>
![alt text](images/Centos/centos9.png)</br>
![alt text](images/Centos/centos10.png)</br>
![alt text](images/Centos/centos11.png)</br>

6.ssh </br>
command:vagrant ssh</br>
root default password :vagrant</br>
![alt text](images/Centos/centos12.png)</br>
![alt text](images/Centos/centos13.png)</br>

</br>
</br>

<a id="docker"></a>
## Docker
</br>
</br>

<a id="nginx"></a>
## Nginx
</br>
</br>

<a id="openresty"></a>
## Openresty
</br>
</br>
<a id="redis"></a>

## Redis
</br>
</br>
<a id="mysql"></a>

## Mysql
</br>
</br>

<a id="gitLab"></a>
## GitLab
</br>
</br>

<a id="jenkins"></a>
## Jenkins
</br>
</br>

<a id="swagger"></a>
## Swagger
</br>
</br>
<a id="springBoot"></a>

## SpringBoot
</br>
</br>

<a id="redisLua"></a>
## Redis+Lua
</br>
</br>

<a id="jmeter"></a>
## Jmeter
</br>
</br>
