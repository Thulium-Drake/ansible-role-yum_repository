## Yum repository, powered by Ansible
This role provides a means to configure a simple Yum repository for use with RedHat-like systems.

It can be installed on either RedHat or Debian and will use Apache as the webserver without authentication.

SSL is a mandatory setting, but you can use self-signed certificates if required.

# Usage
* Install the role (either from Galaxy or directly from GitHub)
* Copy the defaults file to your inventory (or wherever you store them) and
  fill in the blanks
* Add the role to your master playbook
* Run Ansible
* ???
* Profit!

# Adding packages
After setting up the repo server you can add packages with the following script:

/usr/local/bin/repo-add [package] [distro_major_version]

There is a sample yum.repo file provided at https://<server>/yum.repo. Any changes made will not be overwritten by Ansible
