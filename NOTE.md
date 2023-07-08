### ssh_config vs sshd_config
In the /etc/ssh file you'll usually find these two files. DO NOT GET THEM MIXED UP!
   - ssh is configuring for the ssh client on your own computer, which is used when you connect with other computers
   - sshd is configuring for the ssh daemon on your computer, which is used when others try to connect to your computer

### /etc/sudoers/ file
A file that allocates system rights to system users. It's basically good for anything you have to do with groups.
