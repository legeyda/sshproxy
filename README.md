

PROXY_ADDRESS=localhost:1081 SSH_ARGUMENTS='-i /home/user/.ssh/staging.legeyda.com/sshproxyuser' SSH_DESTINATION=sshproxyuser@staging.legeyda.com sh run install 


	ssh -vvNTD localhost:1081 -o 'ServerAliveInterval 60' -i ~/.ssh/staging.legeyda.com/sshproxyuser sshproxyuser@staging.legeyda.com