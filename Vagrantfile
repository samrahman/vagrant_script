# -*- mode: ruby -*-
# vi: set ft=ruby :
#Scothbox

Vagrant.configure("2") do |config|
  config.vm.box_url = "/media/sami/DATA/Downloads/vagrantbox/scotch.box"
  config.vm.box = "scotch/box"
  config.vm.hostname = "scotchbox"
  
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.network "public_network"
  #config.vm.network :forwarded_port, guest: 80, host: 8080
  
  
  #config.vm.synced_folder "/home/sami/projects", "/var/www/public", :mount_options => ["dmode=777", "fmode=666"], 
  #owner: "www-data", group: "www-data"
  config.vm.provision "shell", :path => "install.sh"
  
end
