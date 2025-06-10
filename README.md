This is a good known G1TLH DX-Spider software http://www.dxcluster.org adapted for FreeBSD operating system.

I use FreeBSD 14.2 with perl (v5.36.3) 2 core CPU 256 MB RAM.  Also work nice on OpenBSD 7.7 perl (v5.40) 2 core cpu 128 MB RAM.
Please remember FreeBSD and OpenBSD is not Linux. FreeBSD not consist support for AX.25, netrom, rose etc protocols in kernel. This version of DX-Spider for tcp/ip telnet nodes only.

Installation
Just use Git
This is the download area for the DX Spider system. Please look at the Installation instructions, before downloading the software.

GIT

Once you have git installed then to use it with an existing spider tree do (for FreeBSD/unix users):

login as the sysop user

  git clone https://github.com/vladshup/DX-spider-FreeBSD-fork.git spider.new
 
  sudo cp -a spider.new /spider
 
  rm -rf spider.new
 
  cd /spider
 
  git reset --hard
 

Next time 

sudo cp /spider/rc.d/spider /etc/rc.d/spider

Add string to /etc/rc.conf

spider_enable="YES"

Also we need to make symlink for perl

 ln -s /usr/local/bin/perl /usr/bin/perl



