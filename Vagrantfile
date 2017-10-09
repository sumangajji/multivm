Vagrant.configure("2") do |config|

 config.vm.define "web" do |web|
 web.vm.box = "ubuntu/trusty64"
 web.vm.hostname = 'web'
 end

 config.vm.define "db" do |db|
 db.vm.box = "aerospike/centos-6.5"
 db.vm.hostname = 'db'
 end

  config.vm.network "public_network"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
  end

     config.vm.define "control" do |control|
     control.vm.box = "ubuntu/trusty64"
     control.vm.hostname = 'control'
     end
end
