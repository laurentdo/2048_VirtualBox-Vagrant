# -*- mode: ruby -*-
# vi: set ft=ruby :
#2048_VirtualBox-Vagrant

Vagrant.configure("2") do |config|
    config.vm.provider "virtualbox" do |vb|
        vb.memory = 512
    end
    config.vm.box = "ubuntu/xenial32"
	
    config.vm.define :master do |master_config|
        master_config.vm.host_name = "master"
        master_config.vm.network "forwarded_port", guest: 80, host: 8080, id: "nginx"
		master_config.vm.provision "shell", inline: <<-SHELL
			sudo apt-get -y update
			sudo apt-get -y install nginx
			sudo rm -R /var/www/html
			sudo git clone https://github.com/ObjectifLibre/2048.git /var/www/html
			sudo service nginx start
		SHELL
	end
end
