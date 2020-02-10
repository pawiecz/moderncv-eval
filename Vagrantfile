# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.synced_folder ".", "/vagrant"
  config.vm.provision "latex", type: :shell, inline: <<-SHELL
    export DEBIAN_FRONTEND=noninteractive
    apt-get update
    apt-get install --assume-yes --quiet texlive-latex-extra texlive-lang-polish
  SHELL
end
