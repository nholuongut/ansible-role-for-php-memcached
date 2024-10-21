# Ansible Role: PHP-Memcached

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

Installs PHP Memcached support on RedHat/CentOS/Debian/Ubuntu.

## Requirements

This role doesn't *explicitly* require Memcached to be installed, but if you don't have the daemon running somewhere (either on the same server, or somewhere else), this role won't be all that helpful. Check out `nholuong.memcached` for a simple role to install and configure Memcached (either on the same server, or separate servers).

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    php_enablerepo: ""

(RedHat/CentOS only) If you have enabled any additional repositories (might I suggest nholuong.repo-epel or nholuong.repo-remi), those repositories can be listed under this variable (e.g. `remi,epel`). This can be handy, as an example, if you want to install the latest version of PHP from Remi's repository.

    php_memcached_package: php-memcached

The package to install for PHP Memcached support. For Debian/Ubuntu and PHP 5.x, use `php5-memcached`.

## Dependencies

  - nholuong.php

## Example Playbook

    - hosts: webservers
      roles:
        - { role: nholuong.php-memcached }

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟
