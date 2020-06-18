# Ansible Role

## Requirements:

- VPC [USING SINGLE PUBLIC SUBNET]
  - SECURITY GROUP
  - ROUTE TABLE
  - INTERNET GATEWAY
  - PUBLIC SUBNET

- EC2 INSTANCE
  - SECURITY GROUP

- JENKINS INSTALLATION
  - UPDATE ALL PACKAGES
  - INSTALL COMPATIBE JAVA
  - DOWNLOAD JENKINS
  - INSTALL JENKINS

## Prerequisites:

- CREATE KEYPAIR TO ASSOCIATE IT WITH EC2 INSTANCE WHEN LAUNCHING EC2 INSTANCE
- SSH-AGENT ADD [FOR ALLOWING SSH-KEYGEN FORWARDING] FROM LOCALHOST

## Change the AWS credentials on the yaml fiels for test or use env variables

## Install ansible with boto3 on a Linux vm

    sudo apt install ansible
    sudo apt install python3-pip
    pip3 install boto boto3

## Setup AWS credentials with the CLI

## Place your ssh file

    ssh-agent bash
    ssh-add ~/.ssh/aws-srvubuntu.pem

## Execute:

    ansible-playbook playbook.yml
