Vagrant.configure("2") do |config|
  config.vm.box = "yungsang/boot2docker"
  config.vm.network "private_network", ip: "192.168.33.10"

  path = ENV["HOME"]
  config.vm.synced_folder path, path, type: "nfs", :mount_options => ['nolock,vers=3,udp,noatime,actimeo=1']

  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--memory", "2048", "--cpus", "2"]
  end
end
