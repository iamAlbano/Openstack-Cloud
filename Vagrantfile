Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.disksize.size = "70GB"
  config.vm.hostname = "Openstack-Cloud"
  config.vm.network "public_network", bridge: "np0s3"
  config.vm.provider "virtualbox" do |v|
    v.memory = 8192
    v.cpus = 2
    v.name = "Openstack-Cloud"
  end
  config.vm.provision "shell", path: "initial-devstack-setup.sh"
end