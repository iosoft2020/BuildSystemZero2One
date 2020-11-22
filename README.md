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
- Download url</br>
>https://www.vagrantup.com/downloads.html

![alt text](images/Vagrant/Vagrant1.PNG)

- install</br>
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
- Download url</br>
>https://www.virtualbox.org/wiki/Downloads

![alt text](/images/Virtualbox/Virtualbox1.PNG?raw=true)

- install</br>
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
- search and confirm centos version from vagrant repository</br>
vagrant repository url:</br>
>https://app.vagrantup.com/boxes/search</br>

![alt text](images/Centos/centos1.png)</br>
![alt text](images/Centos/centos2.png)</br>

- init centos </br>

>vagrant init centos/7

![alt text](images/Centos/centos3.png)</br>
![alt text](images/Centos/centos4.png)</br>

- open C:\Users\xxxx and confirm Vagrantfile</br>
![alt text](images/Centos/centos5.png)</br>

- edit Vagrantfile for specify the memory size and ip</br>

>  config.vm.provider "virtualbox" do |vb| </br>
>     vb.memory = "2048"                   </br>
>  end </br>
>
>  config.vm.network "private_network", ip: "192.168.56.66"</br>

![alt text](images/Centos/centos6.png)</br>

- auto download centos and start </br>

>vagrant up

![alt text](images/Centos/centos7.png)</br>
![alt text](images/Centos/centos8.png)</br>
![alt text](images/Centos/centos9.png)</br>

- ssh </br>

>vagrant ssh

root default password 
>vagrant

![alt text](images/Centos/centos10.png)</br>
![alt text](images/Centos/centos11.png)</br>

- increase disk size on a Vagrant VM using VirtualBox
![alt text](images/Centos/centos12.png)</br>
![alt text](images/Centos/centos13.png)</br>
![alt text](images/Centos/centos14.png)</br>
![alt text](images/Centos/centos15.png)</br>

>"C:\Program Files\Oracle\VirtualBox\VBoxManage.exe" clonehd centos-7-1-1.x86_64.vmdk centos-7-1-1.x86_64_clone.vdi --format vdi</br>

![alt text](images/Centos/centos16.png)</br>
![alt text](images/Centos/centos17.png)</br>

>"C:\Program Files\Oracle\VirtualBox\VBoxManage.exe" modifyhd centos-7-1-1.x86_64_clone.vdi compact</br>

![alt text](images/Centos/centos18.png)</br>

>"C:\Program Files\Oracle\VirtualBox\VBoxManage.exe" modifyhd centos-7-1-1.x86_64_clone.vdi --resize 307200</br>

![alt text](images/Centos/centos19.png)</br>

>"C:\Program Files\Oracle\VirtualBox\VBoxManage.exe" clonehd centos-7-1-1.x86_64_clone.vdi centos-7-1-1.x86_64_vdi_2_vmdk.vmdk --format vmdk</br>

![alt text](images/Centos/centos20.png)</br>
![alt text](images/Centos/centos21.png)</br>
![alt text](images/Centos/centos22.png)</br>
![alt text](images/Centos/centos23.png)</br>
![alt text](images/Centos/centos24.png)</br>
![alt text](images/Centos/centos25.png)</br>
![alt text](images/Centos/centos26.png)</br>
![alt text](images/Centos/centos27.png)</br>
![alt text](images/Centos/centos29.png)</br>

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
