## Pre-activity: Installing your Server

For us to have a same environment we will install our server using a kickstart file that is provided in this training.

First click start to the VM

![alt text][pre11-StartingVM]

Click the folder in the right side and locate your Centos ISO that we downloaded earlier then click start

![alt text][pre12-Choose]

While starting keep pressing up button to avoid timeout and wait that screen is like this:

![alt text][pre13-QuickUP]

Then press the Tab button and add append after the `quiet` this line ` ks=https://goo.gl/pWp15s`

It output will be like this:

![alt text][pre14-Kickstart]

Then press enter.

After 5-10 mins You will see a screen like this:

![alt text][pre15-Installing]

This means it the server is installing this will take a while, after installation you will see this screen:

![alt text][pre16-Reboot]

Before you press reboot remove first the ISO by clicking on Menu Tab > Devices > Optical Drives > Remove disk from virtual drives (Force Unmount if needed)

Then Click Reboot

(If The Vm takes time to reboot just click in Menu tab > Machine > Reset)

If you successfully followed all the steps you can Login with this credentials:

Username: `student` Password: `linux101`

[pre11-StartingVM]: https://github.com/ajohnsc/L101/blob/master/pictures/pre11-StartingVM.PNG

[pre12-Choose]: https://github.com/ajohnsc/L101/blob/master/pictures/pre12-Choose.PNG

[pre13-QuickUP]: https://github.com/ajohnsc/L101/blob/master/pictures/pre13-QuickUP.PNG

[pre14-Kickstart]: https://github.com/ajohnsc/L101/blob/master/pictures/pre14-Kickstart.PNG

[pre15-Installing]: https://github.com/ajohnsc/L101/blob/master/pictures/pre15-Installing.PNG

[pre16-Reboot]: https://github.com/ajohnsc/L101/blob/master/pictures/pre16-Reboot.PNG
