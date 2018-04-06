# Gitlab runner host

Creates an EC2, installs Docker, aws cli and a vanilla Gitlab runner for simple builds. Option to install other runner types.


> Read more about Gitlab runners <a href="https://docs.gitlab.com/ee/ci/runners/" target="_blank">here</a>

## Installing the runners
1. Run the `gitlabrunner-host.yml` in the AWS console with the following parameters:
### Network Configuration
* The VPC and subnet
* Cidr block for an IP to access from if you want to SSH into the host.
### Host Settings
* KeyName for the SSH
### Runner Settings
* Runner name. A friendly name for your runner
* `GitLabRegistrationToken` GitLab registration token from one of your repositories (repo -> Settings -> CI/CD -> Runner settings -> Registration token under specific runners).
* `GitlabServer` The Gitlab master to connect to. Defaults to https://gitlab.com. Change if you have an internal enterprise Gitlab you want to connect to.





    