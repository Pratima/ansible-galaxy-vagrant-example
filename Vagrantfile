Vagrant.require_version '>= 1.8.1'

Vagrant.configure(2) do |config|
  config.vm.box_url = "https://github.com/2creatives/vagrant-centos/releases/download/v6.5.3/centos65-x86_64-20140116.box"
  config.vm.box = "centos-6.5.3"

  config.vm.define 'nginxDemo' do |box|
    box.vm.hostname = 'nginxDemo'
    box.vm.network :private_network, ip: '10.0.0.11'
    box.vm.network :forwarded_port, guest: 22, host: 2211, id: 'ssh'
  end

end
