Vagrant.configure("2") do |config|
  ## Chose your base box
  config.vm.box = "precise64"

 
  ## For masterless, mount your salt file root
  config.vm.synced_folder "salt/roots/", "/srv/"

  ## Use all the defaults:
  config.vm.provision :salt do |salt|
    salt.minion_config = "salt/minion"
    salt.run_highstate = true
  end
end
