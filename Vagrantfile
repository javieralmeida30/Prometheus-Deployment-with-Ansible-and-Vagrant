Vagrant.configure("2") do |config|
config.vm.box = "geerlingguy/centos7"

config.vm.define "ansiblecontroller" do |ansiblecontroller|
ansiblecontroller.vm.hostname = "ansiblecontroller"
ansiblecontroller.vm.network "forwarded_port", guest: 80, host: 8080
ansiblecontroller.vm.network "private_network", ip: "192.168.56.10"
ansiblecontroller.vm.network "public_network"
end

config.vm.box = "geerlingguy/centos7"

config.vm.define "node1" do |node1|
node1.vm.hostname = "node1"
node1.vm.network "private_network", ip: "192.168.56.11"

end
end
