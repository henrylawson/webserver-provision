VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.box = "utopic"

    config.vm.hostname = "vagrant-webserver"
    config.vm.network "public_network", ip: "192.168.1.31"

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
    end
end