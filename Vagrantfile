
Vagrant.configure("2") do |config|
  
  #config.vm.synced_folder "/home/hardeep/Documents/importprojects/ansibleplaybooks/", "/foo"
  
  config.vm.define "machine1" do |machine1|
    machine1.vm.box = "centos/7"
    config.vm.network "private_network", ip: "192.168.21.10"
    machine1.vm.hostname = "machine1"
  end

  config.vm.define "machine2" do |machine2|
    machine2.vm.box = "centos/7"
    config.vm.network "private_network", ip: "192.168.21.20"
    machine2.vm.hostname = "machine2"
  end

  config.vm.define "controller" do |controller|
    controller.vm.box = "centos/7"
    config.vm.network "private_network", ip: "192.168.21.100"
    controller.vm.hostname = "controller"
  end
end
