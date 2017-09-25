# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "bento/ubuntu-16.04"

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  # eg. You can connect to Service Fabric Explorer at http://192.168.50.50:19080/Explorer.
  config.vm.network "private_network", ip: "192.168.50.50"

  # Share an additional folder to the guest VM. The first argument is
  # the path on the host to the actual folder. The second argument is
  # the path on the guest to mount the folder. And the optional third
  # argument is a set of non-required options.
  # config.vm.synced_folder "../data", "/vagrant_data"

  # We recommend allocating at least 3GB to the Service Fabric onebox environment
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "3072"
  end

  # Copy Java libraries to shared host folder to enable local build
  #config.vm.provision "shell", inline:
  #  $script

  config.vm.define :ServiceFabric do |t|
  end
end
