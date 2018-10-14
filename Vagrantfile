Vagrant.configure("2") do |config|
  config.vm.box = "mikrotik-routeros-6.38.5"
  config.vm.provision "ansible" do |ansible|
    ansible.compatibility_mode = '2.0'
    ansible.playbook = "playbook.yml"
    ansible.extra_vars = {
      mikrotik_hostname: "router",
    }
  end
end
