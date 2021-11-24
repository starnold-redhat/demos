*Please note the details of this demo is for internal red hat uk only, however the broad steps could be done by anyone.  The requirements are to have satellite and a rhel vm.*

# Prepare the vm to be managed by insights

Create a new virtual machine using the ansible tower in demolab

ssh onto the new machine

Install the insights-client - `sudo dnf install insights-client`

UPgrade to RHEL 8.4 - `sudo dnf update`

Reboot the vm - `sudo reboot`

Then install the compliance packages

`sudo dnf install scap-security-guide openscap-scanner  openscap`


# Configure the vm in satelite so that remote execution will work

In satellite, go to hosts, search for your host

Click on the host name

Click on edit host in the top corner

Click on the ansible roles tab, click on "ansible Roles" and then click submit

Click on edit - then ckcik on manage host, click on submit.
