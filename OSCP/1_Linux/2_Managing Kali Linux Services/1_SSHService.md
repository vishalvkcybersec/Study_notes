The secure shell service is most commonly used to remotely access a computer using a secure encrypted protocol.

The SSH service is TCP based and listens by default on port 22.

To start ssh service, run systemctl with the start option followed by the service name.
sudo systemctl start ssh


To verifyif the ssh service is working by running the coomand

sudo ss -antlp | grep sshd


To start the ssh service automatically at boottime after changing the default kali passwd, we pass systemctl the enable parameter

sudo systemctl enable ssh