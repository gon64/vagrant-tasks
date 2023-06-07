Vagrant.configure("2") do |config|

  config.vm.define "dev" do |dev|
    dev.vm.box = "debian/bullseye64"
    dev.vm.hostname = "vagrant-dev"
    dev.vm.provision "shell", path: "provision.sh"
    dev.vm.provision "shell", path: "provision-dev.sh"
    #dev.vm.network "public_network", ip: "192.168.1.100"
    dev.vm.network "forwarded_port", guest: 80, host: 8181
  end

  config.vm.define "sta" do |sta|
    sta.vm.box = "debian/bullseye64"
    sta.vm.hostname = "vagrant-sta"
    sta.vm.provision "shell", path: "provision.sh"
    sta.vm.provision "shell", path: "provision-sta.sh"
    #sta.vm.network "public_network", ip: "192.168.1.200"
    sta.vm.network "forwarded_port", guest: 80, host: 8282
  end

end