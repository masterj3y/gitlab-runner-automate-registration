Vagrant.configure("2") do |config|
  config.vm.define "gitlab_runner" do |gitlab_runner|
    gitlab_runner.vm.box = "generic/debian12"

    gitlab_runner.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yaml"
    end
  end

  config.vm.provision "file", source: "~/.ssh/id_rsa_server.pub", destination: "~/.ssh/id_rsa_server.pub"
  config.vm.provision "shell", inline: <<-SHELL
    cat /home/vagrant/.ssh/id_rsa_server.pub >> /home/vagrant/.ssh/authorized_keys
  SHELL
end
