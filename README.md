# Ansible playbook

## Prerequisites
  - Python
  - pip
  - botocore
  - boto3
  - Ansible
    
## Summary
The Ansible playbook should create an EC2 instance and open its SSH port 22. Afterward, it installs Nginx on the VM and creates a sample webpage. The webpage uses javascript to display the current time as taken from [here](https://www.w3schools.com/js/tryit.asp?filename=tryjs_timing_clock).

## Steps
1. Set up the environment variables
2. Create EC2 instance
3. Print its IP address
4. Edit the security group to open port 22
5. Install Nginx
6. Start Nginx
7. Save the html webpage in the command

## Usage
Run `ansible-playbook playbook.yml`

## References
https://medium.com/@a_tsai5/creating-an-ec2-instance-using-ansible-764cf70015f6
https://docs.ansible.com/ansible/latest/collections/amazon/aws/ec2_instance_module.html
https://www.w3schools.com/js/tryit.asp?filename=tryjs_timing_clock
