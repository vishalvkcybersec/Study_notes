The apache HTTP service is often used for a penetration test either for hosting a site or providing a platform for downloading files to a victim machine.

The HTTP service is TCP based and listens by default on port 80.

To start the HTTP service on kali, we can use 

sudo systemctl start apache2

To verify that the htttp service is running and listening on TCP port 80 with ss and grep

sudo ss -antlp | grep apache

To have the http service to start at boottime, we need to run the command
sudo systemctl enable apache2


Most services in kali Linux are operated in much the same way as ssh and http through their service or init scripts.


To see a list of all the available services
systemctl list-unit-files