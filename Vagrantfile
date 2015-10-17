# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure(2) do |config|

  config.vm.hostname  = "docker"
  config.vm.box = "ubuntu/trusty64"
  config.vm.provision "shell", inline: $script

  # config.vm.synced_folder ".", "/opt/app"
end

$script = <<SCRIPT
echo I am provisioning...
date > /etc/vagrant_provisioned_at
SCRIPT
