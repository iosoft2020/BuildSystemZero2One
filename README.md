# BuildSystemZero2One
- [Vagrant](#vagrant)
  - [Download](#vagrant_download)
  - [Install](#vagrant_install)
- [Oracle VM Virtualbox](#virtualbox)
  - [Download](#virtualbox_download)
  - [Install](#virtualbox_install)
- [Centos(Vagrant+Oracle VM Virtualbox)](#centos)
- [Docker](#docker)
- [Nginx](#nginx)
- [Openresty](#openresty)
- [Redis](#redis)
- [Mysql](#mysql)
- [GitLab](#gitLab)
- [Jenkins](#jenkins)
- [Swagger](#swagger)
- [SpringBoot](#springBoot)
- [Redis+Lua](#redisLua)
- [Jmeter](#jmeter)

<a id="vagrant"></a>
## Vagrant

<a id="vagrant_download"></a>
- Download</br>
Download url</br>
>https://www.vagrantup.com/downloads.html

![alt text](images/Vagrant/Vagrant1.PNG)
<a id="vagrant_install"></a>
- Install</br>
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
<a id="virtualbox_download"></a>
- Download</br>
Download url</br>
>https://www.virtualbox.org/wiki/Downloads

![alt text](/images/Virtualbox/Virtualbox1.PNG?raw=true)

<a id="virtualbox_install"></a>
- Install</br>
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

- edit Vagrantfile for specify the disk and the memory size and ip</br>

>  config.disksize.size = '300GB'</br>
>  config.vm.provider "virtualbox" do |vb| </br>
>     vb.memory = "2048"                   </br>
>  end </br>
>
>  config.vm.network "private_network", ip: "192.168.56.66"</br>

![alt text](images/Centos/centos6.png)</br>

- Vagrant install vagrant-disksize plugin</br>
>vagrant plugin install vagrant-disksize

![alt text](images/Centos/centos7.png)</br>
![alt text](images/Centos/centos8.png)</br>

- auto download centos and start </br>

![alt text](images/Centos/centos9.png)</br>

>vagrant up</br>

![alt text](images/Centos/centos10.png)</br>
![alt text](images/Centos/centos11.png)</br>
![alt text](images/Centos/centos12.png)</br>

- Confirm resize status </br>

![alt text](images/Centos/centos13.png)</br>

- Ssh and use root login </br>

>vagrant ssh</br>

![alt text](images/Centos/centos14.png)</br>

>su root</br>
root default password </br>
>vagrant</br>

![alt text](images/Centos/centos15.png)</br>

- format the new disk
>df -hT</br>

![alt text](images/Centos/centos17.png)</br>
![alt text](images/Centos/centos18.png)</br>

>fdisk -l</br>

![alt text](images/Centos/centos19.png)</br>
![alt text](images/Centos/centos20.png)</br>

>fdisk /dev/sda</br>

![alt text](images/Centos/centos21.png)</br>

>d</br>

![alt text](images/Centos/centos22.png)</br>

>n</br>

![alt text](images/Centos/centos23.png)</br>

>p</br>

![alt text](images/Centos/centos24.png)</br>

>Enter key</br>

![alt text](images/Centos/centos25.png)</br>

>Enter key</br>

![alt text](images/Centos/centos26.png)</br>

>Enter key</br>

![alt text](images/Centos/centos27.png)</br>

>p</br>

![alt text](images/Centos/centos28.png)</br>

>w</br>

![alt text](images/Centos/centos29.png)</br>
![alt text](images/Centos/centos30.png)</br>

>rebbot</br>

![alt text](images/Centos/centos31.png)</br>

>df -hT</br>

![alt text](images/Centos/centos32.png)</br>
![alt text](images/Centos/centos33.png)</br>

>xfs_growfs / -d</br>

![alt text](images/Centos/centos34.png)</br>
![alt text](images/Centos/centos35.png)</br>

>df -hT</br>

![alt text](images/Centos/centos36.png)</br>
![alt text](images/Centos/centos37.png)</br>


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
