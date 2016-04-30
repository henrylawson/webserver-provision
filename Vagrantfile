VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.hostname = "vagrant-webserver"
  config.vm.network :private_network, ip: "192.168.3.10"
  config.hostsupdater.aliases = [
    "foinq.com",
    "www.foinq.com",
    "foinq.com.au",
    "www.foinq.com.au",
    "bookeye.foinq.com",
    "hen3rz.com",
    "henrylawson.net",
    "www.henrylawson.net"
  ]

  config.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
  end
end
