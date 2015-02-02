
This file lists how the Chef Push Jobs project is maintained. When making changes to the system,
this file tells you who needs to review your patch - you need a simple majority of
maintainers for the relevant subsystems to provide a :+1: on your pull request. Additionally,
you need to not receive a veto from a Lieutenant or the Project Lead.

Check out [How Chef is Maintained](https://github.com/opscode/chef-rfc/blob/master/rfc030-maintenance-policy.md#how-the-project-is-maintained) for details on
the process, how to become a maintainer, lieutenant, or the project lead.

# Project Lead

* [Mark Anderson](http://github.com/manderson26)

# Core Components

#### Server
* [omnibus-pushy](http://github.com/chef/omnibus-pushy): Configuration for the Chef Push Jobs Server
  installation, and the [Omnibus](http://github.com/chef/omnibus) project definition for building it.
* [opscode-pushy-server](http://github.com/chef/opscode-pushy-server) The erlang push jobs service.
* [pushy-server-schema](https://github.com/chef/pushy-server-schema) The database schema
* [oc-pushy-pedant](http://github.com/chef/oc-pushy-pedant) Tests for the push jobs system.

#### Client
* [omnibus-chef](http://github.com/chef/omnibus-chef): Configuration for the Chef Push Jobs Client
  installation, and the project defintion for it and chef.
* [opscode-pushy-client](http://github.com/chef/opscode-pushy-client) The ruby push jobs client

#### Knife extensions
* [knife-push](https://github.com/chef/knife-push) Knife extensions to use the push jobs service.

### Lieutenants

### Maintainers

