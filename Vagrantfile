Vagrant.configure("2") do |config|
    config.vm.provider :virtualbox do |v|
      v.memory = 2048
      v.cpus = 2
    end

    config.vm.define :master do |master|
      # Vagrant va récupérer une machine de base ubuntu 20.04 (focal) depuis cette plateforme https://app.vagrantup.com/boxes/search
      master.vm.box = "ubuntu/focal64"
      master.vm.hostname = "master"
      master.vm.network :private_network, ip: "10.10.0.10"
    end
  end