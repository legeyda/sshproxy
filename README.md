

	SSHPROXY_USER=user SSHPROXY_GROUP=user SSHPROXY_LISTEN_ADDRESS=localhost:1081 SSHPROXY_SSH_ARGUMENTS='-i /home/user/.ssh/y.legeyda.com/sshproxyuser' SSHPROXY_CONNECT_ADDRESS=sshproxyuser@y.legeyda.com bash run install


	ssh -vvNTD localhost:1081 -o 'ServerAliveInterval 60' -i ~/.ssh/staging.legeyda.com/sshproxyuser sshproxyuser@staging.legeyda.com


	sudo bash -c ". $HOME/box/etc/sshproxy/x.legeyda.com.env && bash run install"
	sudo bash -c ". $HOME/box/etc/sshproxy/t1-laptop.env && bash run install"