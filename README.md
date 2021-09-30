DAY 0 OPERATIONS WITH F5 + VSPHERE + AAP
========================================

Overview
--------

Day 0 operations are a huge part of delivering applications to your private cloud.  This code will help anyone who is looking to try to deploy BIG-IP Platform on vSphere using Ansible Automation Platform (AAP).  Being able to deploy fast demonstration environments to production all it takes is the flip of a switch.

The Day 0 Operations with F5 + vSphere + AAP delivers a few different scenarios

-	Singular or Multiple - Lab Deployments of BIG-IP in HA Pair using Linked Clones
-	Singular or Multiple - Production Deployments of BIG-IP in HA Pair using Full Clones
-	Application Tenant Deployments via AS3 into the above deployed environments

Prerequisites
-------------

-	Ansible Automation Platform - Tested in 2.0, should be backwards compatible to Tower and AAP 1.0
-	vSphere Environment - Tested in 7.x environments, should work fine in 6.7+
-	BIG-IP Image - Recommend 16.1 as it provisions the fastest due to extra configuraitons not being needed
-	BIG-IQ License Server - This code utilizes BIG-IQ License Server and Pools to license and unlicense BIG-IPs using Declaritive Onboarding
-	Enable Exposure for access to /awx/ via the AAP Settings --> Job Settings --> "Paths to expose to isolated jobs"
-	Make sure to modify and copy the vars files in a location that is accessable to the ansible automation platform environment (in my use case i create /awx/vars/ on the AAP 2.0 server and used that for my vault file and deployment yaml files)
-	For my test scenarios i also created /awx/files/ and stored my BIG-IP OVA on in that location to be called from my deployments.yaml (vars file)

Where to get Started?
---------------------

-	Watch my AnsibleFest presenation to see how all of the code works (will upload to youtube soon)
-	Take - Fork - Expand! - Please feel free to use this for your own environment!
