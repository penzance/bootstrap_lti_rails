Vagrant::Config.run do |config|
  config.vm.box       = 'precise64'
  config.vm.box_url   = 'http://files.vagrantup.com/precise64.box'
  config.vm.host_name = 'rails-web-dev-box'

  config.vm.forward_port 3000, 3000
  config.vm.forward_port 8000, 8000
  config.ssh.forward_agent = true
  #config.vm.customize ["modifyvm", :id, "--natdnsproxy1", "off"]

  config.vm.customize ["modifyvm", :id, "--memory", 1024]

  #config.vm.provision :puppet,
  #  :manifests_path => 'puppet/manifests',
  #  :module_path    => 'puppet/modules',
  #  :manifest_file  => 'default.pp',
  #  :options        => '--verbose'
end