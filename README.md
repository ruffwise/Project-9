# Project-9 CI Pipeline for Tooling Website.

### Install Jenkins server

`sudo apt update`

`sudo apt-get install openjdk-11-jdk-headless`

`wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -`

`sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'`

`sudo apt update`

`sudo apt-get install jenkins`
![](/images/jenkins.png)

### configure jenkins to retrieve source-code from GitHub using webhooks

![](/images/console-output.png)

### configure triggering job from webhook

![](/images/configure-trigger.png)

![](/images/artifact.png)

### CONFIGURE JENKINS TO COPY FILES TO NFS SERVER VIA SSH

Install "publish over SSH" plugin
![](/images/publish-over-ssh.png)

![](/images/post-build.png)
