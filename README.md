# GitHub中国加速访问

### 问：为什么访问速度会很慢

- - - - -

### 答：GitHub的CDN域名遭到DNS污染
GitHub在中国大陆访问速度慢的问题原因有很多，但最直接和最主要的原因是GitHub的分发加速网络的域名遭到DNS污染。

由于GitHub的加速分发CDN域名assets-cdn.github.com遭到DNS污染，导致无法连接使用GitHub的加速分发服务器，才使得中国大陆访问速度很慢。

### 问：如何解决DNS污染
- - - - -
### 答：通过修改Hosts解决污染问题

一般的DNS问题都可以通过修改Hosts文件来解决，GitHub的CDN域名被污染问题也不例外，同样可以通过修改Hosts文件解决。

将域名解析直接指向IP地址来绕过DNS的解析，以此解决污染问题。


### 问：如何修改Hosts文件
- - - - - -
### 答：请按以下步骤操作
* 访问[IPAddress.com](https://www.ipaddress.com/ip-lookup)使用IP Lookup工具获得这个域名的IP地址。
* 修改系统的Hosts文件
### host文件存放位置

 + 类unix

   >etc/hosts

 + Windows
  
   > C:\Windows\System32\drivers\etc\hosts

 
