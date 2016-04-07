# freezer-scheduler-service
This is a simple systemd service script to start and stop OpenStack Freezer Scheduler services.

# Centos 7 Installation

First let's copy "freezer.env" file to "/run" directory.

Than configure "freezer.env" file. There is enough information in the file:

	vi /run/freezer.env
    
Copy "freezer-scheduler.service" file to "/usr/lib/systemd/system/"

	vi /usr/lib/systemd/system/freezer-scheduler.service
    
Start the service

	systemctl start freezer-scheduler
    
Enable the service to start on boot:

	systemctl enable freezer-scheduler