Vagrant.configure("2") do |config|
  (1..3).each do |i|
    config.vm.define "debian#{i}" do |machine|
      machine.vm.box = "debian12"
      machine.vm.network "public_network", bridge: "enp2s0"
      machine.vm.provider "virtualbox" do |vb|
        vb.memory = "2048"
        vb.cpus = 2
      end
    end
  end
end