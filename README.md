# ansible-role-php-fpm
Ansible role to install PHP on OpenResty / NGINX. OpenResty / NGINX **should** be installed.
This role is intended to be used with [WordPress](https://github.com/HauptJ/ansible-role-wordpress) and [Redis](https://github.com/HauptJ/ansible-role-redis).

[![Build Status](https://travis-ci.org/HauptJ/ansible-role-php-fpm.svg?branch=master)](https://travis-ci.org/HauptJ/ansible-role-php-fpm)

## Installation
1. Fork this repository
2. git submodule add <git host> roles/ansible-role-php-fpm
    - [submodule reference](https://chrisjean.com/git-submodules-adding-using-removing-and-updating/)

**Ansible Galaxy:** [HauptJ.php-fpm](https://galaxy.ansible.com/HauptJ/php-fpm/)


## Variables

### PHP FPM

| Name 						                  | Default 							                    | Description 										        |
|-----------------------------------|-------------------------------------------|-----------------------------------------|
| php_sock                          | /var/run/wordpress.sock                   | PHP socket address                      |
| resty_web_user                    | nginx                                     | OpenResty web service user and group    |
| resty_default_web_dir             | /usr/local/openresty/nginx/html/default   | web directory                           |
