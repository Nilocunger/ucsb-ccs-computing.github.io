$script = <<-SCRIPT
apt-get update
apt-get install -y curl ruby dirmngr
SCRIPT

$rvm = <<-SCRIPT
gpg --keyserver hkp://pool.sks-keyservers.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
\\curl -sSL https://get.rvm.io | bash -s stable --ruby
SCRIPT

Vagrant.configure("2") do |config|
  config.vm.box = "bento/debian-9.6"
  config.vm.provision "shell", inline: $script
  config.vm.provision "shell", inline: $rvm, privileged: false
  config.vm.provision "shell", inline: "cd /vagrant && ./setup.sh", privileged: false
  config.vm.network "forwarded_port", guest: 4000, host: 4000, host_ip: "127.0.0.1"
end
