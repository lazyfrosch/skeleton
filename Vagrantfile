# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = 'ubuntu-trusty-server-amd64'
  config.vm.box_url = 'https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box'
  config.vm.hostname = 'mailserver.example.org'

  config.vm.provision 'puppet' do |puppet|
    puppet.manifests_path = 'vagrant'
    puppet.modules_path = '../'
    #puppet.options = '--modulepath /vagrant/spec/fixtures/modules --verbose --debug'
  end

end