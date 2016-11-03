# data-as-a-service
This repository contains components necessary to create a Data as a Service (DaaS) layer that allows clients to attach to one data service to access many data at rest repositories on the back end. Red Hat JBoss Data Virtualization (JDV) allows you to easily combine data from multiple, heterogenous data sources without moving or copying any data. This project uses JDV to create the DaaS and Red Hat Mobile Application Platform (RHMAP) running within OpenShift Container Platform to create a mobile client.

The following is done by running ansible script (which will be included in this repo shortly)...

 1. Install & Configure JBoss Data Virtualization - 5 minutes

    Download the Quick-Start Kit. https://developers.redhat.com/download-manager/file/dv_quickstart-2.1.0-dist.zip

    Unzip the Quick-Start kit.

    Open the terminal and change your present working directory(pwd) to home folder of Quick-Start kit.

    Run setup_dv.sh (.bat) script. This will:

        Install and Start Red Hat JBoss Data Virtualization 6.3 server with default settings.

        Start H2 database server and populate with sample datasource for Getting Started example.

        Configure and deploy Web Service.
 2. Set Up Dev Environment - 5 minutes

    Install the Java SE Development Kit (JDK), we recommend OpenJDK or Oracle JDK 1.8 or above.

    Download Red Hat JBoss Developer Studio

    Run Red Hat JBoss Developer Studio installer

        For MAC/Linux:

            Go to the folder where you have downloaded Red Hat JBoss Developer Studio, and execute the installer

            java -jar jboss-devstudio-9.1.0.GA-installer-eap.jar

            Note: This will execute the Red Hat JBoss Developer Studio installation wizard.

        For Windows:

            Right Click on jboss-devstudio-9.1.0.GA-installer-eap.jar

            Select Open With >Jar Launcher

    Install JBoss Developer Studio Integration Stack (JBDSIS) plugins

        Start Red Hat JBoss Developer Studio.

        In Red Hat JBoss Developer Studio, click Help > Red Hat Central action from the main menu.

        Click the tab Software/Update and select the JBoss Data Virtualization Development option and then click Install

        Note: If Red Hat JBoss Data Virtualization Development is already installed then proceed to next step. You can confirm that JBDSIS is installed on your machine by clicking What is already installed link.

        Note: If you are facing proxy issues downloading JBDSIS plugins via Red Hat Central, then you can download JBDSIS plugins locally to your computer from this link.

        Click Next.

        Accept any additional dependencies and license agreements, and then click Finish to complete.

Note: When installation is complete you will be prompted to re-launch Red Hat JBoss Developer Studio to ensure the new features are fully operational.
