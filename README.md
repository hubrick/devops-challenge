# Hubrick DevOps Challenge

Your objective is to create a [Chef] cookbook that provisions and configures an Ubuntu instance, running nginx that serves a plain html hello world file on port 80.

For setting up the cookbook structure and handling the chef dependencies use [Berkshelf]. Local provisioning and testing shall be handled with [Test Kitchen] – you can use either the default [Vagrant] driver or [Docker] driver for this. Provide at least one spec using [InSpec] that ensures the correct setup of the instance.

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

* Use the [EC2] driver instead of Vagrant/Docker to provision an AWS instance.
* Integrate [travis-ci] in your solution's repository to run the tests automatically.

[Chef]: https://www.chef.io/
[Berkshelf]: https://docs.chef.io/berkshelf.html
[Test Kitchen]: http://kitchen.ci/
[InSpec]: https://www.inspec.io/
[Vagrant]: https://www.vagrantup.com/
[Docker]: https://github.com/test-kitchen/kitchen-docker
[EC2]: https://github.com/test-kitchen/kitchen-ec2
[travis-ci]:  https://travis-ci.org/
