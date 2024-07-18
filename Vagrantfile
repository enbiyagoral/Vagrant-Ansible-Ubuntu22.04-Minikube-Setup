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
  
  config.vm.define "minikube" do |minikube|
    minikube.vm.box = "ubuntu/jammy64"
    minikube.vm.network "private_network", ip: "192.168.56.13"
    minikube.vm.hostname = "minikube"

    minikube.vm.provider "virtualbox" do |vb|
      vb.memory = "4096"
    end
  end
end
