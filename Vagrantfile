# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.require_version ">= 1.6.5"

Vagrant.configure(2) do |config|
  config.vm.define "app" do |app|
    app.vm.provider "docker" do |d|
      d.build_dir = "."
      d.vagrant_vagrantfile = "Vagrantfile.proxy"
      d.has_ssh = true
    end
    # Sync the project directory using rsync
    app.vm.synced_folder ".", "/home/vagrant/vagrant-docker-dev", type: "rsync"
  end
end
