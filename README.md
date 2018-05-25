# Linux 101

This is a training prepared to understand Linux and how to administer it.

In this training you only need the following:
- VirtualBox
- Centos ISO

## Pre Activity : Setting up your VM

1.) Download and install VirtualBox

You can download VirtualBox by clicking [here](https://www.virtualbox.org/wiki/Downloads)

2.) Download CentOS ISO

You can download your Latest Centos ISO [here](https://www.centos.org/download/)

Then click Minimal ISO to dowload the appropirate image

3.) Setup your VM in your VirtualBox

Open VirtualBox

![alt text][pre01-VirtualBox]

Create a new VM by clicking New

![alt text][pre02-CreateVM]

Click on Expert mode to fasten the process

![alt text][pre03-ExpertMode]

Fill it up by the following:

|Field|Value|
|---|---|
|Name|Linux 101|
|Type|Linux|
|Version|Red Hat (64 bit)|
|Memory Size|4096 MB|
|Hard Disk|Create a virtual disk now|


Then Click Create to create the Virtual disk:

|Field|Value|
|---|---|
| File location | Linux 101 |
| File Size | 20 GB |
| Hard disk file type | VDI (VirtualBox Disk Image) |
| Storage on physical hard disk | Dynamically Allocated |


Then click Create and you have successfully created your VM now we just need some few changes in network settings

![alt text][pre06-VMSample]

Click Setting

![alt text][pre07-Settings]

Click Network

![alt text][pre08-Network]

Change the network settings of the First Adapter with the following settings:

|Field|Value|
|---|---|
|Enable Network Adapter| Checked |
|Attached to:|Host-only Adapter|
|Name:|VirtualBox Host-Only Ethernet adapter|

![alt text][pre09-Adapter1]

Now we need to configure your second Adapter by clicking Adapter and use the following settings:

|Field|Value|
|---|---|
|Enable Network Adapter| Checked |
|Attached to:|NAT|

![alt text][pre10-Adapter2]

Then Click OK

You have finally set-up your VM now we will install your server,Click [here](https://github.com/ajohnsc/L101/blob/master/activities/README.md)


[pre01-VirtualBox]: https://github.com/ajohnsc/L101/blob/master/pictures/pre01-VirtualBox.PNG "Sample Opened VirtualBox"

[pre02-CreateVM]: https://github.com/ajohnsc/L101/blob/master/pictures/pre02-CreateVM.PNG
"It will popout simillar like this"

[pre03-ExpertMode]: https://github.com/ajohnsc/L101/blob/master/pictures/pre03-ExpertMode.PNG


[pre05-Storage]: https://github.com/ajohnsc/L101/blob/master/pictures/pre05-Storage.PNG

[pre06-VMSample]: https://github.com/ajohnsc/L101/blob/master/pictures/pre06-VMSample.PNG

[pre07-Settings]: https://github.com/ajohnsc/L101/blob/master/pictures/pre07-Settings.PNG

[pre08-Network]: https://github.com/ajohnsc/L101/blob/master/pictures/pre08-Network.PNG

[pre09-Adapter1]: https://github.com/ajohnsc/L101/blob/master/pictures/pre09-Adapter1.PNG

[pre10-Adapter2]: https://github.com/ajohnsc/L101/blob/master/pictures/pre10-Adapter2.PNG
