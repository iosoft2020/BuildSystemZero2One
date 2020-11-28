# BuildSystemZero2One
- [Vagrant](#vagrant)
  - [Download](#vagrant_download)
  - [Install](#vagrant_install)
- [Oracle VM Virtualbox](#virtualbox)
  - [Download](#virtualbox_download)
  - [Install](#virtualbox_install)
- [Centos(Vagrant+Oracle VM Virtualbox)](#centos)
  - [Search and confirm centos version from vagrant repository](#centos_search_and_confirm_centos_version_from_vagrant_repository)
  - [Init centos](#centos_init_centos)
  - [Open user dir and confirm Vagrantfile](#centos_open_user_dir_confirm_Vagrantfile)
  - [Edit Vagrantfile for specify the disk and the memory size and ip](#centos_edit_Vagrantfile_for_specify_the_disk_and_the_memory_size_and_ip)
  - [Install vagrant-disksize plugin](#centos_install_vagrant_disksize_plugin)
  - [Auto download centos and start](#centos_auto_download_centos_and_start)
  - [Confirm resize status](#centos_confirm_resize_status)
  - [Ssh and use root login](#centos_ssh_and_use_root_login)
  - [Format the new disk](#centos_format_the_new_disk)
- [Docker](#docker)
  - [Remove default docker](#docker_remove_default_docker)
  - [Install dependent package](#docker_install_dependent_package)
  - [Set docker download repository](#docker_set_docker_download_repository)
  - [Update yum package index](#docker_update_yum_package_index)
  - [Install docker](#docker_install_docker)
  - [Start docker when system start](#docker_start_docker_when_system_start)
  - [Start docker](#docker_start_docker)
  - [Confirm docker version](#docker_confirm_docker_version)
- [Nginx](#nginx)
- [Openresty](#openresty)
- [Redis](#redis)
- [Mysql](#mysql)
- [GitLab](#gitLab)
- [Jenkins](#jenkins)
- [Swagger](#swagger)
  - [Maven dependency](#swagger_maven_dependency)
  - [Localhost Url](#swagger_localhost_url)
  - [Configuretion Class](#swagger_configuretion_class)



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
<a id="centos_search_and_confirm_centos_version_from_vagrant_repository"></a>
- Search and confirm centos version from vagrant repository</br>
vagrant repository url:</br>
>https://app.vagrantup.com/boxes/search</br>

![alt text](images/Centos/centos1.png)</br>
![alt text](images/Centos/centos2.png)</br>

<a id="centos_init_centos"></a>
- Init centos </br>

>vagrant init centos/7

![alt text](images/Centos/centos3.png)</br>
![alt text](images/Centos/centos4.png)</br>

<a id="centos_open_user_dir_confirm_Vagrantfile"></a>
- Open C:\Users\xxxx and confirm Vagrantfile</br>
![alt text](images/Centos/centos5.png)</br>

<a id="centos_edit_Vagrantfile_for_specify_the_disk_and_the_memory_size_and_ip"></a>
- Edit Vagrantfile for specify the disk and the memory size and ip</br>

>  config.disksize.size = '300GB'</br>
>  config.vm.provider "virtualbox" do |vb| </br>
>     vb.memory = "2048"                   </br>
>  end </br>
>
>  config.vm.network "private_network", ip: "192.168.56.66"</br>

![alt text](images/Centos/centos6.png)</br>

<a id="centos_install_vagrant_disksize_plugin"></a>
- Install vagrant-disksize plugin</br>
>vagrant plugin install vagrant-disksize

![alt text](images/Centos/centos7.png)</br>
![alt text](images/Centos/centos8.png)</br>

<a id="centos_auto_download_centos_and_start"></a>
- Auto download centos and start </br>

![alt text](images/Centos/centos9.png)</br>

>vagrant up</br>

![alt text](images/Centos/centos10.png)</br>
![alt text](images/Centos/centos11.png)</br>
![alt text](images/Centos/centos12.png)</br>

<a id="centos_confirm_resize_status"></a>
- Confirm resize status </br>

![alt text](images/Centos/centos13.png)</br>

<a id="centos_ssh_and_use_root_login"></a>
- Ssh and use root login </br>

>vagrant ssh</br>

![alt text](images/Centos/centos14.png)</br>

>su root(root default password:vagrant)</br>

![alt text](images/Centos/centos15.png)</br>

<a id="centos_format_the_new_disk"></a>
- Format the new disk
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

>reboot</br>

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

<a id="docker_remove_default_docker"></a>
- Remove default docker
>yum remove docker docker-common docker-selinux docker-engine</br>

![alt text](images/Docker/docker1.png)</br>
![alt text](images/Docker/docker2.png)</br>

<a id="docker_install_dependent_package"></a>
- Install dependent package
>yum install -y yum-utils device-mapper-persistent-data lvm2</br>

![alt text](images/Docker/docker3.png)</br>
![alt text](images/Docker/docker4.png)</br>
![alt text](images/Docker/docker5.png)</br>

<a id="docker_set_docker_download_repository"></a>
- Set docker download repository
>yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo</br>

![alt text](images/Docker/docker6.png)</br>
![alt text](images/Docker/docker7.png)</br>

<a id="docker_update_yum_package_index"></a>
- Update yum package index
>yum makecache fast</br>

![alt text](images/Docker/docker8.png)</br>
![alt text](images/Docker/docker9.png)</br>

<a id="docker_install_docker"></a>
- Install docker
>yum install docker-ce</br>

![alt text](images/Docker/docker10.png)</br>
![alt text](images/Docker/docker11.png)</br>
![alt text](images/Docker/docker12.png)</br>
![alt text](images/Docker/docker13.png)</br>

<a id="docker_start_docker_when_system_start"></a>
- Start docker when system start
>systemctl enable docker</br>

![alt text](images/Docker/docker14.png)</br>

<a id="docker_start_docker"></a>
- Start docker
>systemctl start docker</br>

![alt text](images/Docker/docker15.png)</br>
![alt text](images/Docker/docker16.png)</br>

<a id="docker_confirm_docker_version"></a>
- Confirm docker version
>docker version</br>

![alt text](images/Docker/docker17.png)</br>
![alt text](images/Docker/docker18.png)</br>

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
<a id="swagger_maven_dependency"></a>
- Maven dependency
>        <dependency></br>
>            <groupId>io.springfox</groupId></br>
>            <artifactId>springfox-swagger2</artifactId></br>
>            <version>2.9.2</version></br>
>        </dependency></br>
>
>        <dependency></br>
>            <groupId>io.springfox</groupId></br>
>            <artifactId>springfox-swagger-ui</artifactId></br>
>            <version>2.9.2</version></br>
>        </dependency></br>

<a id="swagger_localhost_url"></a>
- Localhost url</br>
>http://localhost:8080/swagger-ui.html

<a id="swagger_configuretion_class"></a>
- Configuretion Class
```java
package com.iosoft2020.MySwagger.config;

import java.util.ArrayList;

import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.core.env.Environment;
import org.springframework.core.env.Profiles;

import springfox.documentation.builders.PathSelectors;
import springfox.documentation.builders.RequestHandlerSelectors;
import springfox.documentation.service.ApiInfo;
import springfox.documentation.service.Contact;
import springfox.documentation.spi.DocumentationType;
import springfox.documentation.spring.web.plugins.Docket;
import springfox.documentation.swagger2.annotations.EnableSwagger2;

@Configuration
@EnableSwagger2
public class MySwaggerConfig {

    @Bean
    public Docket docker(Environment environment) {

        Profiles profiles = Profiles.of("dev", "test");
        environment.acceptsProfiles(profiles);

        return new Docket(DocumentationType.SWAGGER_2).apiInfo(apiInfo())
                //				.enable(environment.acceptsProfiles(profiles))
                .groupName("group1")
                .select()
                // withMethodAnnotation
                .apis(RequestHandlerSelectors.basePackage("com.iosoft2020.MySwagger.controller"))
                //				.paths(PathSelectors.ant("/iosoft2020/**"))
                .build();
    }

    @Bean
    public Docket dockerGroupA(Environment environment) {

        return new Docket(DocumentationType.SWAGGER_2).apiInfo(apiInfo())
                //				.enable(environment.acceptsProfiles(profiles))
                .groupName("groupA")
                .select()
                // withMethodAnnotation
                .apis(RequestHandlerSelectors.basePackage("com.iosoft2020.MySwagger.controller"))
                .paths(PathSelectors.ant("/iosoft2020/**"))
                .build();
    }

    private ApiInfo apiInfo() {

        Contact contack = new Contact("iosoft2020", "https://github.com/iosoft2020/BuildSystemZero2One",
                "xxx@xxx.com");

        return new ApiInfo("MySwaggerAPI Document", "MySwaggerApi", "1.0",
                "https://github.com/iosoft2020/BuildSystemZero2One/blob/main/README.md#swagger",
                contack, "Apache 2.0", "http://www.apache.org/licenses/LICENSE-2.0",
                new ArrayList<>());
    }
}
```




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
