# concource-examples

Examples using Concource.ci.

## Install

```bash
$ git clone git@github.com:jkamenik/concourse-examples.git
$ cd concourse-examples
$ vagrant up

# log into concourse CLI
# Note: the target name of "example" is required
$ fly -t example login -c http://192.168.100.4:8080

# install all examples
$ bin/install

# install a specific example
$ bin/install hello-world
```

The UI is running at 192.168.100.4:8080.

> Example are not started by default.
