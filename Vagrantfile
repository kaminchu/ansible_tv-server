Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-18.04"


  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
    ansible.inventory_path = "development"
    ansible.limit = 'all'
  end
end
