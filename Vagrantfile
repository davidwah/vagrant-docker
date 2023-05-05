Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-22.04"
  config.vm.box_version = "202206.13.0"
  config.vm.hostname = "node-demo"
  config.vm.provision "shell", path: "get-docker.sh"
  config.vm.network "public_network", bridge: "wlp3s0"
  config.vm.provider :virtualbox do |vb|
    vb.memory = 1024
    vb.cpus = 1
  end
end
