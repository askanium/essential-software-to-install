# essential-software-to-install

A list of software to install on a new machine or on a newly installed OS (I used everything to install on a Linux Mint 18.1) for a web developer and machine learning practitioner.

## As of 2016-12-21

- [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
- [oh-my-zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md)
- [Python 3](http://python.org)
- `$ sudo apt-get install python-dev python3-dev` (dev headers for python2 and python3)
- pip / pip3 (`sudo apt-get install python-pip python3-pip`)
- [virtualenvwrapper](http://virtualenvwrapper.readthedocs.io/en/latest/install.html)
- [Sublime Text](http://www.sublimetext.com/3) / [Atom](https://atom.io/) / [Notepad++](https://notepad-plus-plus.org/)
- IDEs: [PyCharm / WebStorm](https://www.jetbrains.com/)
- [nodejs / npm](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)
- `$ sudo npm install -g gulp grunt`
- chromium (from Application Store / repo)
- git (`$ sudo apt-get install git`)
- [JRE / JDK](https://www.digitalocean.com/community/tutorials/how-to-install-java-on-ubuntu-with-apt-get)
- Shutter (for screenshots from Application Store)
- [VirtualBox](https://www.virtualbox.org/wiki/Linux_Downloads)
- `$ sudo apt-get install ruby-dev` to install ruby dev headers (needed to install compass below)
- `$ gem install compass`

### Docker

- [Docker Engine](https://docs.docker.com/engine/installation/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Docker Machine](https://docs.docker.com/machine/install-machine/)

### Databases

#### PostgreSQL
- [PostgreSQL 9.6](https://raonyguimaraes.com/how-to-install-postgresql-9-6-on-ubuntudebianlinux-mint/) ([configuration](https://help.ubuntu.com/community/PostgreSQL) note that postgresql is already installed) **Note:** after installing it using described method, I found out that it is actually available in the Application Store (on Linux Mint)
- `$ sudo apt-get install postgresql-server-dev-9.6` (needed for pgAdmin 4)
- [pgAdmin4](https://www.pgadmin.org/download/pip4.php) (if install fails, try running `sudo apt-get install libpq-dev python-dev libxml2-dev libxslt1-dev libldap2-dev libsasl2-dev libffi-dev`)
- add alias to run from terminal on `pgadmin` (`echo "alias pgadmin=\"workon pgadmin-env && python ~/.virtualenvs/pgadmin-env/lib/python3.5/site-packages/pgadmin4/pgAdmin4.py\"" >> .zshrc
`) adjust for virtualenv name and python version

#### MySQL
- MySQL-server 5.7.16 from Application Store (on Mint)
- MySQL-workbench from Application Store (on Mint)
- If you are using MySQL wiht python, install `sudo apt-get install libmysqlclient-dev`, otherwise `MySQL-python` package will throw an error on install (`mysql_config` not found)

# Linux settings

## Privacy

- [disable IPv6](https://www.linuxbabe.com/ubuntu/disable-ipv6-on-ubuntu) if the VPN does not offer IPv6 leak protection
