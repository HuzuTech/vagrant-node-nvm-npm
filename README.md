#Vagrant-Node-Nvm-Npm

This is a setup for a Vagrant box with node, nvm and npm installed. It
should be useful for testing node apps in a greenfield environment.

To create a box of your own:

- Get [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- Get [Vagrant](http://http://downloads.vagrantup.com/)
- Install Chef:  
  ```gem install chef``` (you will need Ruby and ruby-dev/devel)
- Install librarian-chef:
  ```gem install librarian-chef```
- Install the necessary Chef cookbooks:
  ```librarian-chef install```
- Add an appropriate Vagrant box:
  ```vagrant box add precise64 http://files.vagrantup.com/precise64.box```

You can now provision and boot your box:
```vagrant up```

To ssh into it as user `vagrant`:
```vagrant ssh```

To exit the box:
```exit```

To destroy the box:
```vagrant destroy```
