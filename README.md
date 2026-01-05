# Fail2Ban Filters and Addons

## fail2ban
Fail2ban is a handy little security solution that bans upon multiple failed access attempts. Available on the EPEL (Extra Packages for Enterprise Linux) repository.
To install, follow these steps:

### Install instructions

+ Install EPEL-RELEASE repository and the fail2ban packages
```
yum install epel-release
yum install fail2ban fail2ban-systemd
```
+ Copy the contents of the repository to `/etc/fail2ban/`
+ Enable fail2ban at boot and start
```
systemctl enable --now fail2ban
```

### Changelog:
+ Added filters for GitLab (13)


[Source](https://gist.github.com/pawilon/238c278d3c6c4669771eb81b03264acd)