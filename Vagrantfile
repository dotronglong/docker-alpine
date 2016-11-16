Vagrant.configure("2") do |config|
  config.vm.box = "dotronglong/alpine"
  config.vm.box_check_update = false
  config.vm.network "private_network", ip: "192.168.69.96"
  config.vm.provision "shell", path: "https://github.com/dotronglong/vagrant-provisioners/raw/master/alpine/latest/docker.sh"
  config.vm.provider "virtualbox" do |vb|
     vb.memory = "4096"
  end
end
