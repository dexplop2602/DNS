# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"
  config.vm.hostname = "debian"
  config.vm.network "private_network", ip: "192.168.56.10"

  config.vm.synced_folder "config/", "/vagrant/config", create: true

  config.vm.provider "virtualbox" do |vb|
  end

  config.vm.provision "shell", path: "bootstrap.sh"
end
