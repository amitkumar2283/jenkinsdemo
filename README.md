# Intro

Chef server acts as a central repository for your Chef code as well as for information about every node it manages.

![image](https://docs.chef.io/_images/start_chef.svg)

A **node** is any computer that is managed by a Chef server.

In practice, you use Chef to manage your servers remotely, typically from a Windows, Mac OS, or Linux workstation. Although you're configuring Red Hat Enterprise Linux or CentOS in this tutorial, your workstation can be any OS you choose.


# Installation:

_INFO_ :  RPM Installation: 
```sh
rpm -Uvh  *RPM package name*```

* Chef Server : https://downloads.chef.io/chef-server/12.11.1
* ChefDK (can be installed on any machine, but is gnerally installed on the Chef server): https://downloads.chef.io/chefdk/1.1.16
* Chef Client : 
 * manual installation (ignore) : https://downloads.chef.io/chef/12.17.44)
 * Bootstrapping : on Chef Server 
```sh
knife bootstrap <node FQDN/IP> -x username -P password --sudo```
 * Verify client is connected post installation: 
 ```sh
 knife client show name_of_node```
  * list all clients : 
  ```sh
  knife client list```



