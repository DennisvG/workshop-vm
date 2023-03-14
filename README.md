# workshop-vm

Workshop in Dutch for setting up a linux virtual environment in [Virtualbox](https://www.virtualbox.org) using [Vagrant](https://www.vagrantup.com).
Installing and configure apache webserver. And Installing and configure a jboss/wildfly application server.

## Workshop 1
Setting up environment

## Workshop 2
Installing and configure apache webserver
TO DO: Rewrite config for apache 2.4

## Workshop 3
Installing and configure a jboss/wildfly application server
You need to download jboss from [Redhat Website](https://developers.redhat.com/products/eap/download) supscription required or [Wildfly](https://www.wildfly.org) 
Using SampleWebApp.war found on [this website](https://www.middlewareinventory.com/blog/sample-web-application-war-file-download/) with some modifications (= included in files)

## Workshop 4
Automate everything with Ansible
Part 1: webserver
Part 2: jboss
Using 3 versions of SampleWebApp:
- SampleWebApp-1.0.0.war => working
- SampleWebApp-1.1.0.war => not deploying
- SampleWebApp-1.2.0.war => gives 404.
