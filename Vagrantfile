Vagrant.configure("2") do |config|

  if Vagrant.has_plugin?("vagrant-vbguest")
    config.vbguest.no_install = true
    config.vbguest.auto_update = false
    config.vbguest.no_remote = true
  end

  config.vm.define :cliente1 do |cliente1|
    cliente1.vm.box = "bento/ubuntu-22.04"
    cliente1.vm.network :private_network, ip: "192.168.100.3"
    cliente1.vm.hostname = "cliente1"
    cliente1.vm.box_download_insecure = true
  end

  config.vm.define :cliente2 do |cliente2|
    cliente2.vm.box = "bento/ubuntu-22.04"
    cliente2.vm.network :private_network, ip: "192.168.100.4"
    cliente2.vm.hostname = "cliente2"
    cliente2.vm.box_download_insecure = true
  end

  config.vm.define :servidor1 do |servidor1|
    servidor1.vm.box = "bento/ubuntu-22.04"
    servidor1.vm.network :private_network, ip: "192.168.100.2"
    servidor1.vm.hostname = "servidor1"
    servidor1.vm.box_download_insecure = true
 end
end
