VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # Use the same key for each machine
  config.ssh.insert_key = false

  config.vm.define "ubuntu1804" do |ubuntu1804|
  ubuntu1804.vm.box = "ubuntu/bionic64"
  ubuntu1804.vm.hostname = "ubuntu1804"
  ubuntu1804.vm.network "private_network", ip: "172.21.0.10", netmask: "255.255.255.0"
  ubuntu1804.vm.provider "virtualbox" do |vb|
    vb.name = "ubuntu1804.vagrant.local"
    vb.customize [
      "modifyvm", :id,
      "--groups", "/vagrant.local",
      "--memory", "256",
      "--cpus", "1"
    ]
  end
  ubuntu1804.vm.provision :ansible do |ansible|
      #ansible.compatibility_mode = "2.0"
      ansible.inventory_path = "./inventory/hosts"
      ansible.playbook = "vagrant-lab-bootstrap.yml"
  end
  end

  config.vm.define "ubuntu1604" do |ubuntu1604|
  ubuntu1604.vm.box = "ubuntu/xenial64"
  ubuntu1604.vm.hostname = "ubuntu1604"
  ubuntu1604.vm.network "private_network", ip: "172.21.0.11", netmask: "255.255.255.0"
  ubuntu1604.vm.provider "virtualbox" do |vb|
    vb.name = "ubuntu1604.vagrant.local"
    vb.customize [
      "modifyvm", :id,
      "--groups", "/vagrant.local",
      "--memory", "256",
      "--cpus", "1"
    ]
  end
  ubuntu1604.vm.provision :ansible do |ansible|
      #ansible.compatibility_mode = "2.0"
      ansible.inventory_path = "./inventory/hosts"
      ansible.playbook = "vagrant-lab-bootstrap.yml"
  end
  end

  config.vm.define "debian9" do |debian9|
  debian9.vm.box = "debian/stretch64"
  debian9.vm.hostname = "debian9"
  debian9.vm.network "private_network", ip: "172.21.0.20", netmask: "255.255.255.0"
  debian9.vm.provider "virtualbox" do |vb|
    vb.name = "debian9.vagrant.local"
    vb.customize [
      "modifyvm", :id,
      "--groups", "/vagrant.local",
      "--memory", "256",
      "--cpus", "1"
    ]
  end
  debian9.vm.provision :ansible do |ansible|
      #ansible.compatibility_mode = "2.0"
      ansible.inventory_path = "./inventory/hosts"
      ansible.playbook = "vagrant-lab-bootstrap.yml"
  end
  end

  config.vm.define "debian8" do |debian8|
  debian8.vm.box = "debian/jessie64"
  debian8.vm.hostname = "debian8"
  debian8.vm.network "private_network", ip: "172.21.0.21", netmask: "255.255.255.0"
  debian8.vm.provider "virtualbox" do |vb|
    vb.name = "debian8.vagrant.local"
    vb.customize [
      "modifyvm", :id,
      "--groups", "/vagrant.local",
      "--memory", "256",
      "--cpus", "1"
    ]
  end
  debian8.vm.provision :ansible do |ansible|
      #ansible.compatibility_mode = "2.0"
      ansible.inventory_path = "./inventory/hosts"
      ansible.playbook = "vagrant-lab-bootstrap.yml"
  end
  end

  config.vm.define "centos7" do |centos7|
  centos7.vm.box = "centos/7"
  centos7.vm.hostname = "centos7"
  centos7.vm.network "private_network", ip: "172.21.0.30", netmask: "255.255.255.0"
  centos7.vm.provider "virtualbox" do |vb|
    vb.name = "centos7.vagrant.local"
    vb.customize [
      "modifyvm", :id,
      "--groups", "/vagrant.local",
      "--memory", "256",
      "--cpus", "1"
    ]
  end
  centos7.vm.provision :ansible do |ansible|
      #ansible.compatibility_mode = "2.0"
      ansible.inventory_path = "./inventory/hosts"
      ansible.playbook = "vagrant-lab-bootstrap.yml"
  end
  end

config.vm.define "centos6" do |centos6|
centos6.vm.box = "centos/6"
centos6.vm.hostname = "centos6"
centos6.vm.network "private_network", ip: "172.21.0.31", netmask: "255.255.255.0"
centos6.vm.provider "virtualbox" do |vb|
  vb.name = "centos6.vagrant.local"
  vb.customize [
    "modifyvm", :id,
    "--groups", "/vagrant.local",
    "--memory", "256",
    "--cpus", "1"
  ]
end
centos6.vm.provision :ansible do |ansible|
    #ansible.compatibility_mode = "2.0"
    ansible.inventory_path = "./inventory/hosts"
    ansible.playbook = "vagrant-lab-bootstrap.yml"
end
end
end
