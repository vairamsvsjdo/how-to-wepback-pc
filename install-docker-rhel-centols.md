https://access.redhat.com/documentation/en-us/red_hat_network_satellite/5.5/html/reference_guide/sect-reference_guide-package_updater-updating_packages_from_the_command_line_with_yum

``` bash
sudo visudo
```

``` sh
## Allows people in group wheel to run all commands
# %wheel        ALL=(ALL)       ALL

## Same thing without a password
%wheel  ALL=(ALL)       NOPASSWD: ALL
```

``` bash
sudo usermod -aG wheel $USER
sudo su -
yum install docker
usermod -aG dockerroot $USER
# file – User group file
/etc/group 
sudo /etc/docker/daemon.json
```

``` json
{
    "live-restore": true,
    "group": "dockerroot"
}
```

``` bash
systemctl start docker
systemctl restart docker
exit
```
``` bash
docker ps
```


