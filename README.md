# Vagrantfile to create an apache httpd server with the latest codeit repository

## Details
* Starts from the [centos/7 Vagrant image](https://app.vagrantup.com/centos/boxes/7)
* Uses Virtualbox provider with port forwarding
* Downloads apache httpd from the [codeit repository](https://codeit.guru)
* Starts apache on 443 (host = 1443) and 80 (host = 1080)

## Usage
Start and test (will display server information)
* `time vagrant up; echo "*****************************"; curl -v -k https://127.0.0.1:1443 > index.html`
