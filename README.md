# Implementation of an E-Commerce System on AWS in an automated way using Terraform and Ansible

![picture with Cloud Project words and the icons for the services used](https://miro.medium.com/v2/resize:fit:720/format:webp/0*G16GrIIluXceOynM.jpg)

In another project based on a real-world scenario, I worked as Cloud Engineer using DevOps, where I created and implemented an e-Commerce MVP (Minimum Viable Product)
on AWS in less than 2 hours and in an automated way using Terraform and Ansible (Infrastructure as Code — IaC).

I provisioned the infrastructure in an automated way using Terraform and Ansible to automate the configuration management process, software installation and package
management of the EC2 instance. I also used Magento, PHP, MySQL, and Redis to complete this project.

![picture with the words Soluction Architecture and a graph showing the project](https://miro.medium.com/v2/resize:fit:720/format:webp/0*NdAh-uAJIS9dbsOX.jpg)

After setting the Terraform files and uploading them to CloudShell, I only had to use a single Terraform Apple to provide the needed architecture on AWS, meeting the
requirements needed by Magento and with security policies already in place.

With the instance already provisioned, it was to prepare them. Ansible was installed on the machine trought a SSH connections. Some adjusts were made to the Ansible 
Playbook to allow it to run quickly, since it was responsible to prepare the instance and install all the needed software.


![picture showing Terminal running Ansible doing the tasks](https://miro.medium.com/v2/resize:fit:720/format:webp/0*3bl1xYM7GbEq4Uhl.png)

After finalizing the process, I’ve proceeded to test the software, but for some reason I wasn’t getting any answer from the instance. I’ve thought I did something wrong on 
Ansible’s settings, and just thinking about redoing all the settings and provisioning anyone would already be calculating the time needed to do it all again. Thanks to the
speed Terraform and Ansible gave me, I didn’t think twice. I applied a Terraform Destroy to delete the instance and start from scratch, being very careful to make sure 
I didn’t make any more mistakes. After running Ansible again, Magento was successfully installed and available trough the public IP, all of that in less than 15 minutes!

![Picture of a browser window showing the e-commerce running](https://miro.medium.com/v2/resize:fit:720/format:webp/0*PIeakZez1dOxXRB2.png)

After the installation, I added a product and made some light customization, to validate the test.

As part of the project’s extra challenge, I utilized Freenom to get a free test domain name. Using Amazon Route 53, I created a hosted zone, configured the server names generated
by the domain and created a record, pointing the test domain name to the instance public IP address, allowing the project to be reached using a common URL.

The entire process was done in under two hours. Terraform and Ansible gives a lot of speed to provide and to configure, allowing greater agility in decision making. Instead of wasting time
to find a minor error, I could choose to redo the project from scratch without losing much time, which would not be possible without these two tools.




