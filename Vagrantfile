# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.host_name = "CentOS7" # Determines 'Build Host' in resulting RPM
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.config_file = "ansible.cfg"
    ansible.compatibility_mode = "2.0"
    # ansible.verbose = true
  end
end
