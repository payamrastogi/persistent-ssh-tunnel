## persistent-ssh-tunnel
### Steps to create persistent ssh tunnel
1. Add USER_TO_RUN_SERVICE, REMOTE_PORT, SSH_USER, REMOTE_PUBLIC_IP
2. Copy ssh-tunnel-persistent.service to /etc/systemd/system
3. Execute the following commands

```shell
$ sudo systemctl daemon-reload
$ sudo systemctl start ssh-tunnel-persistent.service
```

#### References:
- https://www.tomshardware.com/how-to/host-public-website-raspberry-pi
- https://confluence.jaytaala.com/display/TKB/Create+a+persistent+SSH+tunnel+between+servers+with+systemd
- https://www.golinuxcloud.com/run-systemd-service-specific-user-group-linux/
- https://superuser.com/questions/1700726/how-to-create-persistent-ssh-connection-between-two-servers-in-systemctl
- https://superuser.com/questions/37738/how-to-reliably-keep-an-ssh-tunnel-open
- https://github.com/rydercalmdown/pi_home_reverse_proxy