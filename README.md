# Chef Push

[![Join the chat at https://gitter.im/chef/chef-push](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/chef/chef-push?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This repository is the central repository for the Chef Push Jobs service.

Currently this repository does not contain any code, as the push jobs code is spread out across
several repositories.

The purpose of this repository is to serve as a central place to report
push jobs issues and to outline how to contribute to the push jobs system. If an issue is known to
be against a specific subsystem, you may file it against that system, but it is always appropriate
to file push system issues here.

If you need to file an issue against another Chef project, you can find a list of projects and where
to file issues in the 
[community contributions section](https://docs.chef.io/community_contributions.html#issues-and-bug-reports)
of the [Chef docs](https://docs.chef.io).

## Components of the Chef Push Jobs Service

Following is a list of key components of the Chef Push Jobs service. This is not yet an exhaustive list.

### Commonly-Modified Components

#### Server
* [omnibus-pushy](http://github.com/chef/omnibus-pushy): Configuration for the Chef Push Jobs Server
  installation, and the [Omnibus](http://github.com/chef/omnibus) project definition for building it.
* [opscode-pushy-server](http://github.com/chef/opscode-pushy-server) The erlang push jobs service.
* [pushy-server-schema](https://github.com/opscode/pushy-server-schema) The database schema
* [oc-pushy-pedant](http://github.com/chef/oc-pushy-pedant) Tests for the push jobs system.

#### Client
* [omnibus-chef](http://github.com/chef/omnibus-chef): Configuration for the Chef Push Jobs Client
  installation, and the project defintion for it and chef.
* [opscode-pushy-client](http://github.com/chef/opscode-pushy-client) The ruby push jobs client
* [push-jobs cookbook](https://github.com/opscode-cookbooks/push-jobs) Push jobs Cookbook


#### Knife extensions
* [knife-push](https://github.com/chef/knife-push) Knife extensions to use the push jobs service.

### Less-Commonly-Modified Components

* [opscode-pushy-simulator](https://github.com/chef/opscode-pushy-simulator) A client simulator in
  erlang used for load testing.
* [pushy-common](https://github.com/chef/pushy_common) Common code between the simulator and the service.

## Major Technologies used in Chef Push Server

* Erlang
* PostgreSQL
* ZeroMQ

If you're looking to contribute to certain parts of the push jobs service, familiarity with the
following related tools is also beneficial, depending on the area.

* rebar (used for dependency management in Erlang)
* sqitch (database migrations)

