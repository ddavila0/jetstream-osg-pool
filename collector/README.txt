Installation instructions for the OSG CE Collector on Jetstream
===============================================================

Follow the instructions in
Buildfile

Used on the Cybera openstack:
https://cloud.cybera.ca/

Deployed as a 
m1.medium instance.

Needs to add security groups to open the follwoing ports:
ssh:22(tcp), squid:3128(tcp), squid:3401(udp)


Pool password file
==================

The instance needs a pool_password file.
It is not part of the github repo for security reasons.
Also notice that this file has to be shared between all the nodes running condor.

If you want to create the pool_password directly in this instance, use
condor_store_cred -f <filename>

