Carbon LightDM Webkit Theme
===========================

This is a theme originally based on <https://github.com/Wattos/LightDM-Webkit-MacOSX-Theme>.

Installation Instructions
-------------------------

You will need LightDM as your login manager. On newer versions of Ubuntu this is already the default. Additionally you will require the webkit greeter. This is done by executing the following command in the command line:

<pre>
sudo apt-get install lightdm-webkit-greeter
</pre>

Once the installation finishes, you need to make the webkit greeter the default greeter. This is done by editing the lightdm configuration under:
 
<pre>
/etc/lightdm/lightdm.conf
</pre>

and changing the greeter-session value to lightdm-webkit-greeter. My lightdm.conf looks like:

[SeatDefaults]
greeter-session=lightdm-webkit-greeter
allow-guest=false
.

The second step is to install the actual theme. This is done by copying the files of this repository into the following location:

<pre>
/usr/share/lightdm-webkit/themes/carbon
</pre>

Finally, change the /etc/lightdm/lightdm-webkit-greeter.conf file to contain the following line: 

<pre>
webkit-theme=carbon
</pre>

Now you can reboot and enjoy the new theme.
