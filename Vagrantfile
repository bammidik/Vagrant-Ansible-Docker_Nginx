Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  
  config.vm.network "public_network", bridge: 'wlp0s20u6', ip: "192.168.1.199"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "provision/playbook.yml"
    ansible.verbose = true
  end

end

