# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "dotronglong/docker-alpine"
  config.vm.box_version = "0.0.1"
  config.vm.box_check_update = false
  config.vm.network "private_network", ip: "192.168.69.96"
  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.provider "virtualbox" do |vb|
     vb.memory = "4096"
  end
end
