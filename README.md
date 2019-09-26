Files:

centos7-cis.ks

minimal.ks

cis-audit


install notes:
    - on bootup, 
Booting Your Kickstart
All the hard work is now done and all that is left to do is to boot off a minimal install CD (or any bootable install media).

Run the automated install by booting from the disk media. When the guests get to the boot screen press the tab key. This allows you to change or add options to the boot configuration.

Simply add the addition content, substituting the IP address for that of the web server in use and the ks.cfg file for the Kickstart file name when the test Kickstart file was created earlier.
<p align="center">
  <img width="75%" src="./readme.images/bootmenu.png">
</p>

   ` vmlinuz initrd=initrd.img ks=https://raw.githubusercontent.com/CoolZeroNL/cissec/master/centos8-cis.ks`




centos7-cis.ks:  kickstart file for CentOS 7, aims to provide a starting point for a Linux admin to build a host which meets the CIS CentOS 7 benchmarks

minimal.ks:  A minimal kickstart file is provided so people can test their setup (PXE/DHCP etc) with a minimal amount of configuration going on.

cis-audit: A bash script to audit whether a host conforms to the CIS benchmarks. 

Aforementioned CIS benchmarks should be able to be found here https://benchmarks.cisecurity.org/tools2/linux/CIS_CentOS_Linux_7_Benchmark_v1.1.0.pdf

I'm not affliated with the Center for Internet Security in any way.
Use any material from this repository at your own risk.  

centos7-cis.ks will need extensive customising to suit a particular user's environment.  There's a lot of config in there because it suits me. e.g. CIS 6.4 /etc/securetty, change it to suit yourself. 


Feel free to get in touch about this.  Particularly with any errors or bugs!

Ross Hamilton <ross.x.hamilton AT gmail.com>
