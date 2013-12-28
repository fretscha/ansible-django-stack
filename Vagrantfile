# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "saucy-server-cloudimg-amd64-vagrant-disk1"
  config.vm.box_url = "http://cloud-images.ubuntu.com/vagrant/saucy/current/saucy-server-cloudimg-amd64-vagrant-disk1.box"

  config.vm.define :webserver1 do |cfg|
    cfg.vm.hostname = "webserver1"
    cfg.vm.network :private_network, ip: "10.110.2.15"
  end

  config.vm.define :dbserver1 do |cfg|
    cfg.vm.hostname = "dbserver1"
    cfg.vm.network :private_network, ip: "10.110.2.16"
  end
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "site.yml"
    ansible.host_key_checking = false
    ansible.verbose = false
  end


end
