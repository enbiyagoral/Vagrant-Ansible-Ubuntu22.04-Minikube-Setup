# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
    ansible.inventory_path = "ansible/inventory.ini"
  end

  config.vm.define "jammy" do |jammy|
    jammy.vm.box = "ubuntu/jammy64"
    jammy.vm.network "private_network", ip: "192.168.56.12"
    jammy.vm.hostname = "jammy"
  end
  
  config.vm.define "minicube" do |minicube|
    minicube.vm.box = "ubuntu/jammy64"
    minicube.vm.network "private_network", ip: "192.168.56.13"
    minicube.vm.hostname = "minicube"

    minicube.vm.provider "virtualbox" do |vb|
      vb.memory = "4096"
    end
  end
end
