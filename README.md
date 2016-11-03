# data-as-a-service
This repository contains components necessary to create a Data as a Service (DaaS) layer that allows clients to attach to one data service to access many data at rest repositories on the back end.  This project uses Red Hat's JBoss Data Virtualization to create the DaaS and Red Hat Mobile Application Platform (RHMAP) running within OpenShift Container Platform to create a mobile client.

The following is done by running ansible script (which will be included in this repo shortly)...

 1. Install & Configure JBoss Data Virtualization - 5 minutes

    Download the Quick-Start Kit. https://developers.redhat.com/download-manager/file/dv_quickstart-2.1.0-dist.zip

    Unzip the Quick-Start kit.

    Open the terminal and change your present working directory(pwd) to home folder of Quick-Start kit.

    Run setup_dv.sh (.bat) script. This will:

        Install and Start Red Hat JBoss Data Virtualization 6.3 server with default settings.

        Start H2 database server and populate with sample datasource for Getting Started example.

        Configure and deploy Web Service.
