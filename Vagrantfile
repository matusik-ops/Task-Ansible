Vagrant.configure("2") do |config|
 
  #Define the first VM
  #login: vagrant ssh vm1

  config.vm.define "vm1" do |vm1|
    vm1.vm.box = "bento/ubuntu-22.04"
    vm1.vm.hostname = "master"
    vm1.vm.network "private_network", ip: "192.168.56.11"
  #vm1.vm.network "public_network", bridge: "wlp3s0"
    vm1.vm.provider "virtualbox" do |vb|
      vb.memory = "4096"
      vb.cpus = 2
    end
  end

 #Define the second VM
  config.vm.define "vm2" do |vm2|
    vm2.vm.box = "bento/ubuntu-22.04"
    vm2.vm.hostname = "worker1"
    vm2.vm.network "private_network", ip: "192.168.56.12"
  #vm2.vm.network "public_network", bridge: "wlp3s0"
    vm2.vm.provider "virtualbox" do |vb|
      vb.memory = "4096"
      vb.cpus = 2
    end
  end
end
