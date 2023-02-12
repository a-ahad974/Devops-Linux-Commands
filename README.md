# Devops-Linux-Commands

Linux is a widely supported, open-source operating system that can run on various computer platforms including x86 and ARM. Its versatility and broad support make it a popular choice for a variety of devices, including computers, servers, mobile devices, and embedded systems. Having a strong understanding of Linux fundamentals and scripting is crucial for a DevOps professional. Many companies rely on Linux as their operating system of choice.

# traceroute
The traceroute tool allows you to track the route that data packets take from your device to a specified endpoint. This endpoint can be identified by its IP address, domain name, or hostname. When using traceroute on the localhost, the results will only show a single hop on the network interface. However, by using traceroute on other IP addresses or domain names, you can see the different routers that data packets pass through on their way to the destination.

root@ubuntu:~ -->> traceroute

# chown

This command enables the user to change the file ownership.

root@ubuntu:~ -->> chown root:root loop.sh

# chmod 

This command allows the user to change the file permissions.

root@ubuntu:~ -->> chmod +x loop.sh

# wget

This command is used for downloading files from the internet. It supports a variety of protocols including HTTP, HTTPS, and FTP. With wget, you can download files, mirror entire websites, and even resume broken downloads.

root@ubuntu:~ -->> wget

# mount

This command is used to mount file systems and devices onto the file system hierarchy. This allows you to access the contents of the file system or device as if it were a local directory on your system.

mount /dev/sdb1 /mnt/data

# df

The df command in Linux is used to display information about the available disk space on the file systems of your system. It shows the total amount of disk space, the used space, and the available space, as well as the percentage of disk space used.

df -h


# ifconfig

This command will allow you to identify all the network interface's IP addresses, MAC addresses, and other details.

root@ubuntu:~ -->> ifconfig

# Firewall 

The Linux kernel's firewall, netfilter, is comprised of two components: the UFW and IPTables. The UFW is responsible for distributing firewall rules to IPTables. UFW is a valuable tool when working with IPTables as it simplifies the process of setting up and managing firewall rules. As an example, the following shows how to permit a connection on port 80 to a web server.

root@ubuntu:~# iptables -A INPUT -p tcp -m tcp --dport 80 -j ACCEPT

root@ubuntu:~# ufw allow 80

# alias

This command in Linux is used to create shortcuts for frequently used commands. An alias is a simple way to refer to a longer command by a shorter name.

alias ll='ls -alF'

# dd

The dd command is utilized for copying and transforming multiple files from various file systems. In recent times, it is predominantly employed for generating a bootable USB drive for Linux. Despite this, there are still numerous other uses for it.

root@ubuntu:~# dd if = /dev/sdb of = /dev/sda
