# spcedge

**Scientific Python, cutting-edge.**

I wanted to have an easy way of spinning up an Ubuntu machine with the latest scientific Python stack installed - so here it is. This will create a virtual machine running 64-bit Ubuntu 14.4 with all the prerequisites for `numpy`, `scipy`, `scikit-learn`, `pandas` and `psycopg2`. These are the packages I needed, but feel free to get in touch if you need more.

## Prerequisites
- [Vagrant](https://www.vagrantup.com/) (tested on 1.7.4),
- [VirtualBox](https://www.virtualbox.org/) (tested on 5.0.0),
- [Ansible](http://www.ansible.com/) (tested on 1.9.4; this dependency means that spcedge does not work natively under Windows - sorry).

## Usage
After cloning the repo, simply:

```
cd spcedge
vagrant up
vagrant ssh
```

You should now be inside a virtual machine that has the basic scientific python packages installed. To start working:

```
source forscience/scripts/activate
```
