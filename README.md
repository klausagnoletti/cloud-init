# cloud-init
Contains cloud-init files I will use to set up various vps for specific needs. For the time of writing this will be for sandboxes relating to tutorial videos.

Each file will contain a use-case.

AWS:
aws ec2 run-instances --image-id ami-0245697ee3e07e755 --count 1 --instance-type t2.nano --key-name MyEC2KeyPair --security-group-ids sg-0c7495e067be12d20 --user-data file:///Users/klaus/Documents/git/cloud-init/tutorialvids-sshbf.yml 

Digital Ocean:
doctl compute droplet create --user-data-file /Users/klaus/Documents/git/cloud-init/tutorialvids-sshbf.yml <instance name>
