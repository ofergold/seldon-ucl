Vagrant.configure(2) do |config|
	config.vm.box = "bandienkhamgalan/seldonucldcs"
	config.vm.box_version = ">=0.7.3"
	config.vm.network :forwarded_port, host: 5000, guest: 80, auto_correct: true
	config.vm.provision :shell, inline: "/home/vagrant/startup.sh", run: "always"
end