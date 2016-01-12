# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "jeqo/centos-7"
  config.vm.box_url = "file:///home/jeqo/boxes/jeqo/centos-7/centos-7.box"

  config.vm.provider "virtualbox" do |vb|
    vb.cpus = 1
    vb.memory = "512"
  end

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "test-install-oracle-java-8-66-centos-7.yml"
  end
end
