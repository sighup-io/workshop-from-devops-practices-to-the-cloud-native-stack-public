# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    {:'macgyver' => {
        :os         => 'bento/ubuntu-18.04',
        :hostname   => 'macgyver',
        :ip         => '192.168.31.31',
        :memory     => '4096',
        :cpus       => 2,
        :autostart  => true,
      },
    }.each do |name, configuration|
      config.vm.define name ,
        primary: configuration[:primary],
        autostart: configuration[:autostart] do |instance|
            if configuration[:os].include?('16.04')
              puts "matching Xenial : #{configuration[:os]} for #{configuration[:name]}"
              instance.cache.synced_folder_opts = {
                  owner: "_apt",
                  group: "_apt",
                  mount_options: ["dmode=777", "fmode=666"]
              }
            end
          instance.vm.box = configuration[:os]
          instance.vm.hostname = configuration[:hostname]
          instance.vm.network 'private_network', ip: configuration[:ip]
          instance.vm.synced_folder "workspace/", "/workspace"

  
          # VirtualBox
          instance.vm.provider 'virtualbox' do |vb|
          # solve https://github.com/hashicorp/vagrant/issues/9524
           vb.name = configuration[:hostname] + "-vm"

          # Boot in headless mode
            vb.gui = false
  
          # VM customization
            vb.cpus = configuration[:cpus]
            vb.customize ['modifyvm', :id, '--memory', configuration[:memory]]
            vb.customize ['modifyvm', :id, '--natnet1', '192.168.199/24']
          end

          instance.vm.provision "shell", path: "https://raw.githubusercontent.com/sighup-io/workshop-from-devops-practices-to-the-cloud-native-stack-public/master/provision.sh"

      end
    end
  end 
