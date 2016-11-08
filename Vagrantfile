Vagrant.configure("2") do |config|
  config.vm.box = "maier/alpine-3.1.3-x86_64"
  config.vm.box_check_update = false
  config.vm.network "private_network", ip: "192.168.69.96"

  # Comment this line after first time machine is up
  config.vm.synced_folder ".", "/vagrant", disabled: true
  # Uncomment below lines after first time machine is up
  # config.vm.synced_folder ".", "/vagrant",
  #  	  :nfs => true,
  #  	  :linux__nfs_options => ['rw', 'no_subtree_check', 'all_squash', 'async']

  config.vm.provider "virtualbox" do |vb|
     vb.memory = "4096"
  end
  config.vm.provision "shell", path: "https://github.com/dotronglong/vagrant-provisioners/raw/master/alpine/latest/docker.sh"
end
