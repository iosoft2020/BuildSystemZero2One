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
- [Openresty(Nginx+Lua)](#openresty)
  - [Install](#openresty_install)
  - [Start openresty when system start](#openresty_start_openresty_when_system_start)
  - [Start openresty](#openresty_start_openresty)
  - [Confirm openresty started](#openresty_confirm_openresty_started)
  - [Embed lua code block](#openresty_embed_lua_code_block)
  - [Embed lua code file](#openresty_embed_lua_code_file)
      - [lua get get request parameters](#openresty_lua_get_get_request_parameters)
      - [lua get post request parameters](#openresty_lua_get_post_request_parameters)
      - [lua get request header parameters](#openresty_lua_get_request_header_parameters)
      - [lua get body parameters](#openresty_lua_get_body_parameters)
- [Lua](#lua)
  - [Confirm version and view install command](#lua_confirm_version_and_view_install_command)
  - [Install Gcc](#lua_install_gcc)
  - [Install](#lua_install)
- [Nginx](#nginx)
  - [Install by docker](#nginx_install_by_docker)
- [Redis](#redis)
- [Mysql](#mysql)
- [GitLab](#gitLab)
- [Jenkins](#jenkins)
- [Swagger](#swagger)
  - [Maven dependency](#swagger_maven_dependency)
  - [Localhost Url](#swagger_localhost_url)
  - [Configuretion(Java)](#swagger_configuretion_java)
  - [Annotation example](#swagger_annotation_example)
      - [Controller](#swagger_annotation_example_controller)
      - [Model](#swagger_annotation_example_model)
  - [UI images](#swagger_ui_images)
  
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

>su root</br>
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

<a id="openresty"></a>
## Openresty(nginx+lua)
<a id="openresty_install"></a>
- Install</br>
>yum install yum-utils

![alt text](images/Openresty/openresty1.png)</br>
![alt text](images/Openresty/openresty2.png)</br>
![alt text](images/Openresty/openresty3.png)</br>
![alt text](images/Openresty/openresty4.png)</br>

>yum-config-manager --add-repo https://openresty.org/package/centos/openresty.repo

![alt text](images/Openresty/openresty5.png)</br>
![alt text](images/Openresty/openresty6.png)</br>

>yum install openresy openresty-resty openresty-opm openresy-doc

![alt text](images/Openresty/openresty7.png)</br>
![alt text](images/Openresty/openresty8.png)</br>
![alt text](images/Openresty/openresty9.png)</br>
![alt text](images/Openresty/openresty10.png)</br>

<a id="openresty_start_openresty_when_system_start"></a>
- Start openresty when system start
>systemctl enable openresty</br>

![alt text](images/Openresty/openresty11.png)</br>
![alt text](images/Openresty/openresty12.png)</br>

<a id="openresty_start_openresty"></a>
- Start openresty
>systemctl start openresty</br>

![alt text](images/Openresty/openresty13.png)</br>
![alt text](images/Openresty/openresty14.png)</br>

<a id="openresty_confirm_openresty_started"></a>
- Confirm openresty started

![alt text](images/Openresty/openresty15.png)</br>

<a id="openresty_embed_lua_code_block"></a>
- Embed lua code block

>cd /usr/local/openresty/nginx/conf/

![alt text](images/Openresty/openresty16.png)</br>

>vi nginx.conf

![alt text](images/Openresty/openresty17.png)</br>


> default_type text/html;</br>
> content_by_lua_block{</br>
>     ngx.say("hello iosoft2020");</br>
> }</br>

![alt text](images/Openresty/openresty18.png)</br>

>systemctl restart openresty

![alt text](images/Openresty/openresty19.png)</br>
![alt text](images/Openresty/openresty20.png)</br>
![alt text](images/Openresty/openresty21.png)</br>

<a id="openresty_embed_lua_code_file"></a>
- Embed lua code file

> mkdir -p /usr/local/openresty/mylua

![alt text](images/Openresty/openresty22.png)</br>

> cd /usr/local/openresty/mylua

![alt text](images/Openresty/openresty23.png)</br>

> vi my.lua

![alt text](images/Openresty/openresty24.png)</br>

> ngx.say("hello iosoft2020 by lua file");

![alt text](images/Openresty/openresty25.png)</br>

> cd /usr/local/openresty/nginx/conf/

![alt text](images/Openresty/openresty26.png)</br>

> vi nginx.conf

![alt text](images/Openresty/openresty27.png)</br>


> \#content_by_lua_block{</br>
> \#ngx.say("hello iosoft2020");</br>
> \#} </br>
> content_by_lua_file /usr/local/openresty/mylua/my.lua;</br>

![alt text](images/Openresty/openresty28.png)</br>

>systemctl restart openresty

![alt text](images/Openresty/openresty29.png)</br>
![alt text](images/Openresty/openresty30.png)</br>
![alt text](images/Openresty/openresty31.png)</br>

<a id="openresty_lua_get_get_request_parameters"></a>
- lua get get request parameters

```lua
-- get uri parameters
local arg = ngx.req.get_uri_args()
for k,v in pairs(arg) do 
    ngx.say("[GET] key:",k," v:",v)
    ngx.say("</br>")
end
```

<a id="openresty_lua_get_post_request_parameters"></a>
- lua get post request parameters

```lua
-- get post parameters
ngx.req.read_body()
local arg = ngx.req.get_post_args()
for k,v in pairs(arg) do 
    ngx.say("[POST] key:",k," v:",v)
    ngx.say("</br>")
end
```

<a id="openresty_lua_get_request_header_parameters"></a>
- lua get request header parameters

```lua
-- get head parameters
local heads = ngx.req.get_headers()
for k,v in pairs(heads) do 
    ngx.say("[HEADER] name:",k," v:",v)
    ngx.say("</br>")
end
```

<a id="openresty_lua_get_body_parameters"></a>
- lua get body parameters

```lua
-- get body parameters
ngx.req.read_body()
local bodydata = ngx.req.get_body_data()
ngx.say(bodydata)
```

<a id="lua"></a>
## Lua
<a id="lua_confirm_version_and_view_install_command"></a>
- Confirm version and view install command</br>
Url</br>
>https://www.lua.org</br>

![alt text](/images/Lua/lua1.png?raw=true)
![alt text](/images/Lua/lua2.png?raw=true)

<a id="lua_install_gcc"></a>
- Install Gcc</br>
>yum -y install gcc</br>
![alt text](/images/Lua/lua3.png?raw=true)
![alt text](/images/Lua/lua4.png?raw=true)

<a id="lua_install"></a>
- Install</br>

>curl -R -O http://www.lua.org/ftp/lua-5.4.2.tar.gz</br>

![alt text](/images/Lua/lua5.png?raw=true)
![alt text](/images/Lua/lua6.png?raw=true)

>tar zxf lua-5.4.2.tar.gz</br>

![alt text](/images/Lua/lua7.png?raw=true)
![alt text](/images/Lua/lua8.png?raw=true)

>cd lua-5.4.2</br>

![alt text](/images/Lua/lua9.png?raw=true)
![alt text](/images/Lua/lua10.png?raw=true)

>make all test</br>

![alt text](/images/Lua/lua11.png?raw=true)
![alt text](/images/Lua/lua12.png?raw=true)

>lua -v</br>

![alt text](/images/Lua/lua13.png?raw=true)
![alt text](/images/Lua/lua14.png?raw=true)

<a id="nginx"></a>
## Nginx
<a id="nginx_install_by_docker"></a>
- Install by docker</br>

>mkdir -p /usr/local/nginx/www /usr/local/nginx/logs /usr/local/nginx/conf</br>

![alt text](/images/Nginx/nginx1.png?raw=true)

>docker pull nginx</br>

![alt text](/images/Nginx/nginx2.png?raw=true)
![alt text](/images/Nginx/nginx3.png?raw=true)

>docker run -d -p 9001:80 --name mynginx nginx</br>

![alt text](/images/Nginx/nginx4.png?raw=true)
![alt text](/images/Nginx/nginx5.png?raw=true)

>docker cp mynginx:/etc/nginx/nginx.conf /usr/local/nginx/conf/mynginx.conf</br>

![alt text](/images/Nginx/nginx6.png?raw=true)

>ll /usr/local/nginx/conf/mynginx.conf</br>

![alt text](/images/Nginx/nginx7.png?raw=true)
![alt text](/images/Nginx/nginx8.png?raw=true)

>docker stop mynginx</br>

![alt text](/images/Nginx/nginx9.png?raw=true)
![alt text](/images/Nginx/nginx10.png?raw=true)

>docker rm mynginx</br>

![alt text](/images/Nginx/nginx11.png?raw=true)
![alt text](/images/Nginx/nginx12.png?raw=true)

> docker run -p 9001:80 --name mynginx \</br>
> -v /usr/local/nginx/www:/usr/share/nginx/html \</br>
> -v /usr/local/nginx/logs:/var/log/nginx \</br>
> -v /usr/local/nginx/conf/mynginx.conf:/etc/nginx/nginx.conf \</br>
> -d nginx</br>

![alt text](/images/Nginx/nginx13.png?raw=true)
![alt text](/images/Nginx/nginx14.png?raw=true)

>docker ps -a</br>
![alt text](/images/Nginx/nginx15.png?raw=true)
![alt text](/images/Nginx/nginx16.png?raw=true)

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

<a id="swagger_configuretion_java"></a>
- Configuretion(Java)
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

<a id="swagger_annotation_example"></a>
- Annotation example

<a id="swagger_annotation_example_controller"></a>
- Controller
```java
package com.iosoft2020.MySwagger.controller;

import java.util.ArrayList;
import java.util.List;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.PostMapping;
import org.springframework.web.bind.annotation.RestController;

import com.iosoft2020.MySwagger.pojo.User;
import com.iosoft2020.MySwagger.response.ErrorResponse;

import io.swagger.annotations.Api;
import io.swagger.annotations.ApiOperation;
import io.swagger.annotations.ApiParam;
import io.swagger.annotations.ApiResponse;
import io.swagger.annotations.ApiResponses;

@RestController
@Api(tags = "Module One API")
public class ModuleOneController {

    @ApiOperation(value = "login", notes = "get username and password")
    @GetMapping("login")
    public String login(@ApiParam("user name") String username, @ApiParam("password") String password) {
        return "welcome. ";
    }

    @ApiOperation(value = "findUser", notes = "find user")
    @ApiResponses(value = {
            @ApiResponse(code = 200, message = "user", response = User.class),
            @ApiResponse(code = 400, message = "invalid parm", response = ErrorResponse.class)
    })
    @PostMapping("findUser")
    public User findUser(String username) {
        return new User();
    }

    @ApiOperation(value = "say hello", notes = "say hello by name")
    @PostMapping("sayHello")
    public String sayHello(@ApiParam("user name") String username) {
        return "hello " + username;
    }

    @ApiOperation(value = "findUsers", notes = "find users")
    @ApiResponse(code = 200, message = "find users", response = User.class, responseContainer = "List")
    @PostMapping("findUsers")
    public List<User> findUsers(String username) {
        return new ArrayList<User>();
    }

}
```

<a id="swagger_annotation_example_model"></a>
- Model
```java
package com.iosoft2020.MySwagger.pojo;

import io.swagger.annotations.ApiModel;
import io.swagger.annotations.ApiModelProperty;

@ApiModel("user pojo")
public class User {

	@ApiModelProperty("user name")
	public String username;

	@ApiModelProperty("password")
	public String password;
}
```

<a id="swagger_ui_images"></a>
- UI images</br>
![alt text](images/Swagger/swagger1.png)</br>
![alt text](images/Swagger/swagger2.png)</br>
![alt text](images/Swagger/swagger3.png)</br>

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
