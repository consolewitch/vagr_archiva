# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/vivid64"
  config.vm.network "private_network", ip: "172.16.0.5"
  config.vm.provision "ansible" do |ansible|
  	ansible.playbook = "ans_archiva/vagrant.yml"
	ansible.vault_password_file = "~/.vault_pass.txt"
  end
end
