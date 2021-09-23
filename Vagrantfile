# vi: set ft=ruby :
Vagrant.configure("2") do |config|

   config.ssh.insert_key= false

   config.vm.define "glusterserver-1" do |node|
       node.vm.box = "centos/7"
       node.vm.hostname = "glusterserver1"
       node.vm.network "private_network", ip: "10.10.0.101"
       node.vm.provider "virtualbox" do |v|
           v.memory = 1024
           v.cpus = 1
        end   

   end

   config.vm.define "glusterserver-2" do |node|
      node.vm.box = "centos/7"
      node.vm.hostname = "glusterserver2"
      node.vm.network "private_network", ip: "10.10.0.102"
      node.vm.provider "virtualbox" do |v|
          v.memory = 1024
          v.cpus = 1
       end   

  end

   config.vm.define "gluster-client" do |node|
       node.vm.box = "centos/7"
       node.vm.hostname = "glusterclient"
       node.vm.network "private_network", ip: "10.10.0.90"
       node.vm.provider "virtualbox" do |v|
           v.memory = 1024
           v.cpus = 1
        end   

   end


end

