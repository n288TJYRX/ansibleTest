# -*- mode: ruby -*-

Vagrant.configure("2") do |config|
config.ssh.insert_key = false
config.vm.provider :virtualbox do |vb|
config.vm.box = "ubuntu/xenial64"
config.vm.network "private_network", ip: "192.168.50.4"
config.vm.network "forwarded_port", guest: 8080, host: 8080, id: "rest-api"
vb.customize ["modifyvm", :id, "--memory", "2048"] end

# Application server 1.
# config.vm.define "app1" do |app|
# app.vm.hostname = "app1.dev"
# app.vm.box = "centos/7"
# app.vm.network "private_network", ip: "192.168.33.10"
# end

end
