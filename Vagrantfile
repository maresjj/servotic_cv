# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.define "webserver-nginx" do |app|
        app.vm.box = "bento/ubuntu-16.04"
        app.vm.network "private_network", ip: "192.168.33.10"
        app.vm.hostname = "webserver-nginx"
        app.vm.provider "virtualbox" do |v|
            v.memory = 1024
            v.cpus = 1
        end
    end
    config.vm.define "dbserver-mysql" do |app|
        app.vm.box = "bento/ubuntu-16.04"
        app.vm.network "private_network", ip: "192.168.33.12"
        app.vm.hostname = "dbserver-mysql"
        app.vm.provider "virtualbox" do |v|
            v.memory = 1024
            v.cpus = 1
        end
    end
end