Vagrant.configure("2") do |config|

  # Define the box and its version
  config.vm.box = "ubuntu/focal64"
  config.vm.box_version = "20240821.0.1"

  # Disable checking for box updates
  config.vm.box_check_update = false

  # Disable the default synced folder
  config.vm.synced_folder ".", "/vagrant", disabled: true

  # Define VM hostname
  config.vm.hostname = "bjit-academy-training-local-vm"

  # Use a private network with a static IP
  config.vm.network "private_network", ip: "192.168.56.150"

  # Specify disk size
  # config.disksize.size = '50GB'

  # Provider-specific configuration
  config.vm.provider "virtualbox" do |vb|
    vb.name = "BJIT Academy"
    vb.memory = 4096
    vb.cpus = 4
  end
end