# Installation

## On Mac

```bash
brew install --cask chef-workstation
```


## On Linux Machine
In order to set up on the Linux machine, we need to first get curl on the machine.

- Step 1 − Once curl is installed on the machine, we need to install Chef on the workstation using Opscode’s omnibus Chef installer.

```bash
$ curl –L https://www.opscode.com/chef/install.sh | sudo bash 
```
- Step 2 − Install Ruby on the machine.

- Step 3 − Add Ruby to path variable.

```bash
$ echo ‘export PATH = ”/opt/chef/embedded/bin:$PATH”’ ≫ ~/.bash_profile && 
source ~/.bash_profile 
```
The Omnibus Chef will install Ruby and all the required Ruby gems into /opt/chef/embedded by adding /opt/chef/embedded/bin directory to the .bash_profile file.

If Ruby is already installed, then install the Chef Ruby gem on the machine by running the following command.

```bash
$ gem install chef 
```

