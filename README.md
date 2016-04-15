# Hubrick DevOps Challenge

Your objective is to create a [Chef] cookbook that provisions and configures a Ubuntu instance, running nginx that serves a plain html hello world file on port 80.

For setting up the cookbook structure and handling the chef dependencies use [Berkshelf]. Local provisioning and testing shall be handled with [Test Kitchen] – you can use the default [Vagrant] driver for this. Provide at least one spec using [Serverspec] that ensures the correct setup of the instance.

## Deliverables

You should provide us with a github repository containing the cookbook. The instance shall be provisioned with the command:
```
$ kitchen converge
```
Tests should be run with:
```
$ kitchen verify
```

### Bonus points

* Use kitchen-ec2 instead of the Vagrant driver to provision an AWS instance.
* Integrate travis-ci in your solution's repository to run the tests automatically.

[Chef]: https://www.chef.io/
[Berkshelf]: http://berkshelf.com/
[Test Kitchen]: http://kitchen.ci/
[Serverspec]: http://serverspec.org/
[Vagrant]: https://www.vagrantup.com/
[travis-ci]:  https://travis-ci.org/
