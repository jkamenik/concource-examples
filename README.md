# concource-examples

Examples using Concource.ci.

## Install

```bash
$ git clone git@github.com:jkamenik/concourse-examples.git
$ cd concourse-examples
$ git checkout docker
$ docker-compose up

# Download the "fly" command from the UI

# log into concourse CLI
# username and password are found in the docker-compose.yml file
# Note: the target name of "example" is required
$ fly -t example login -c http://127.0.0.1:8080

# install all examples
$ bin/install

# install a specific example
$ bin/install hello
```

The UI is running at localhost:8080.

> Example are not started by default.

## Secure data

Things like passwords and keys are provided via variable injection,
and explained in the pipeline files that require them.  Provide keys
and values in a `private.yml` file.

``` yaml
---
git_private_key: ssh-rsa ...
foo: bar
```

## Resources

* [Concourse.io](https://concourse.ci)
* [Concourse Examples](https://github.com/starkandwayne/concourse-tutorial)
