# freezer-scheduler-service
This is a simple systemd service script to start and stop OpenStack Freezer Scheduler services.

# Centos 7 Installation

First let's copy "freezer.env" file to "/run" directory.

Than configure "freezer.env" file. There is enough information in the file:

.. code:: bash

	vi /run/freezer.env
    
Copy "freezer-scheduler.service" file to "/usr/lib/systemd/system/"

.. code:: bash

	vi /usr/lib/systemd/system/freezer-scheduler.service
    
Start the service

.. code:: bash

	systemctl start freezer-scheduler
    
Enable the service to start on boot:

.. code:: bash

	systemctl enable freezer-scheduler