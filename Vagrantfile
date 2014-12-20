VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.box = "utopic"

    config.vm.network :forwarded_port, host: 8080, guest: 80
    config.vm.network :forwarded_port, host: 8443, guest: 443

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
    end
end