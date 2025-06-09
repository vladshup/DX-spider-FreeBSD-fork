This is a good known G1TLH DX-Spider software http://www.dxcluster.org adapted for FreeBSD operating system.S

I use FreeBSD 14.2 with perl (v5.36.3). 
Please remember FreeBSD is not Linux. FreeBSD not consist support for AX.25, netrom, rose etc protocols in kernel. This version of DX-Spider for tcp/ip telnet nodes only.

Installation
Just use Git
This is the download area for the DX Spider system. Please look at the Installation instructions, before downloading the software.

GIT
Git is a complete replacement for CVS. It is the source code management system used for the Linux kernel. It has a many more tools than CVS, amongst which are some source code management visualisation programs. One of these is a Web interface. The web interface to the DXSpider Git repository is available here.

Using Git is quite easy, if you are on a Linux/Unix box. Most distributions have ready made Git packages available. For example Fedora calls the package 'git' (yum install git), Ubuntu and debian call theirs 'git-core' (apt-get install git-core). There is a windows version of Git available on the Google Code site. Just use the full installer which is usually the first one in the list. The others do something different.

Once you have git installed then to use it with an existing spider tree do (for FreeBSD/unix users):-

login as the sysop user

  git clone https://github.com/vladshup/DX-spider-FreeBSD-fork.git spider.new
 
  sudo cp -a spider.new /spider
 
  rm -rf spider.new
 
  cd /spider
 
  git reset --hard
 

Next time 

#sudo cp /spider/rc.d/spider /etc/rc.d/spider

Add string to /etc/rc.conf

spider_enable="YES"

Also we need to make symlink for perl

 ln -s /usr/local/bin/perl /usr/bin/perl



