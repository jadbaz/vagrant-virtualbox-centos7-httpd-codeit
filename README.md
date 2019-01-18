# Vagrantfile to create an apache httpd server from the codeit repository

## Details
* Starts from the [centos/7 Vagrant image](https://app.vagrantup.com/centos/boxes/7)
* Uses Virtualbox provider with port forwarding
* Downloads apache httpd from the [codeit repository](https://codeit.guru)
* Starts apache on 443 (host = 1443) and 80 (host = 1080)

## Usage
Clone, start and test (will display server information)
* `git clone https://github.com/jadbaz/vagrant-virtualbox-centos7-httpd-codeit`
* `cd vagrant-virtualbox-centos7-httpd-codeit`
* `time vagrant up; echo "*****************************"; curl -v -k https://127.0.0.1:1443 > index.html`
