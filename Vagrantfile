# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"

  config.vm.define "web-server" do |web|
    web.vm.network "private_network", ip: "192.168.56.100"
    web.vm.hostname = "web-server"
    web.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = "1"
    end
  end

  config.vm.define "api-server" do |api|
    api.vm.network "private_network", ip: "192.168.56.101"
    api.vm.hostname = "api-server"
    api.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = "1"
    end
  end

  config.vm.define "db-server" do |db|
    db.vm.network "private_network", ip: "192.168.56.102"
    db.vm.hostname = "db-server"
    db.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = "1"
    end
  end
end