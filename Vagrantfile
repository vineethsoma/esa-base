# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure(2) do |config|

	config.vm.box = "esa-base"
	config.vm.hostname="esa02.esadvisory.com"

	config.vm.box_check_update = false
	config.ssh.insert_key=false
	config.ssh.username = 'vagrant'
	config.ssh.password = 'vagrant'
	config.ssh.forward_x11=true

	config.vm.network "public_network"

	config.vm.synced_folder "/disk1/lcm", "/lcm"

	config.vm.provider "virtualbox" do |vb|

		#   vb.gui = true
		vb.cpus = 4

		vb.memory = "4096"
	end

end
