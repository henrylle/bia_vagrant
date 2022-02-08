# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure('2') do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.box = 'ubuntu/focal64'

  # Disable automatic box update checking. If you disable this, then
  # boxes will only be checked for updates when the user runs
  # `vagrant box outdated`. This is not recommended.
  # config.vm.box_check_update = false

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine. In the example below,
  # accessing "localhost:8080" will access port 80 on the guest machine.
  # NOTE: This will enable public access to the opened port
  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine and only allow access
  # via 127.0.0.1 to disable public access
  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  # config.vm.network "private_network", ip: "192.168.33.10"

  # Create a public network, which generally matched to bridged network.
  # Bridged networks make the machine appear as another physical device on
  # your network.
  # config.vm.network "public_network"

  # Share an additional folder to the guest VM. The first argument is
  # the path on the host to the actual folder. The second argument is
  # the path on the guest to mount the folder. And the optional third
  # argument is a set of non-required options.
  # config.vm.synced_folder "../data", "/vagrant_data"

  # Provider-specific configuration so you can fine-tune various
  # backing providers for Vagrant. These expose provider-specific options.
  # Example for VirtualBox:
  #  
  config.vm.network 'forwarded_port', guest: 3001, host: 3001
  config.vm.network 'forwarded_port', guest: 8080, host: 8080
  config.vm.network 'forwarded_port', guest: 5433, host: 5433

  #config.vm.provision 'shell', inline: "sudo sed -i 's/^# deb/deb/g' /etc/apt/sources.list"
  # config.vm.provision 'shell', inline: 'sudo apt-get -y update'

  # # INSTALANDO DOCKER
  # config.vm.provision 'shell', inline: 'sudo apt-get install -y ca-certificates curl gnupg lsb-release'
  # config.vm.provision 'shell',
  #                     inline: 'curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg'
  # config.vm.provision 'shell', inline: 'echo \
  # "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  # $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null'
  # config.vm.provision 'shell', inline: 'sudo apt-get -y update'
  # config.vm.provision 'shell', inline: 'sudo apt-get install -y docker-ce docker-ce-cli containerd.io'

  # # Startando e habilitando docker para já iniciar ativo
  # config.vm.provision 'shell', inline: 'sudo systemctl enable docker.service'
  # config.vm.provision 'shell', inline: 'sudo systemctl enable containerd.service'

  # # Configurando permissão para não ter que ficar usando root
  # config.vm.provision 'shell', inline: 'sudo usermod -aG docker vagrant'
  # config.vm.provision 'shell', inline: 'newgrp docker'

  # # Instalando docker-compose
  # config.vm.provision 'shell',
  #                     inline: 'sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose'
  # config.vm.provision 'shell', inline: 'sudo chmod +x /usr/local/bin/docker-compose'

  # # Instalando o Node
  # config.vm.provision 'shell', inline: 'curl -fsSL https://deb.nodesource.com/setup_14.x | sudo -E bash -'
  # config.vm.provision 'shell', inline: 'sudo apt-get install -y nodejs'
  # # Atualizando versao do NPM
  # config.vm.provision 'shell', inline: 'sudo npm install -g npm@latest --loglevel=error'

  # # Instalando AWS CLI
  # # Pre-requisito (unzip)
  # config.vm.provision 'shell', inline: 'sudo apt-get install unzip -y'

  # # AWS CLI (Install)
  # config.vm.provision 'shell',
  #                     inline: 'curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"'
  # config.vm.provision 'shell', inline: 'unzip awscliv2.zip'
  # config.vm.provision 'shell', inline: 'sudo ./aws/install'

  # # Paradas de teclado br
  # config.vm.provision 'shell', inline: 'sudo loadkeys br'
  # config.vm.provision 'shell', inline: 'sudo apt-get install -y gnome-session gdm3'
  # config.vm.provision 'shell', inline: "sudo sed -i 's/XKBLAYOUT=\"us\"/XKBLAYOUT=\"br\"/g' /etc/default/keyboard"
  # config.vm.provision 'shell',
  #                     inline: 'sudo apt-get install -y virtualbox-guest-dkms virtualbox-guest-utils virtualbox-guest-x11'
  # config.vm.provision 'shell', inline: 'sudo shutdown -r now'

  #
  # View the documentation for the provider you are using for more
  # information on available options.

  # Enable provisioning with a shell script. Additional provisioners such as
  # Ansible, Chef, Docker, Puppet and Salt are also available. Please see the
  # documentation for more information about their specific syntax and use.
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
