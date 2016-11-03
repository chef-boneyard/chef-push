# Chef Push

This is the central repository for the Chef Push Jobs service.

This repository does not contain any code, as the push jobs code is spread out across
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

### Server

* [opscode-pushy-server](http://github.com/chef/opscode-pushy-server) The Erlang push jobs service.

### Client

* [opscode-pushy-client](http://github.com/chef/opscode-pushy-client) The Ruby push jobs client as
  well as its installation configuration and project definition.
* [push-jobs cookbook](https://github.com/opscode-cookbooks/push-jobs) Push jobs cookbook.

### Knife plugins

* [knife-push](https://github.com/chef/knife-push) Knife plugin to use the push jobs service.

### Common Components

* [opscode-pushy-simulator](https://github.com/chef/opscode-pushy-simulator) A client simulator in
  erlang used for load testing.
* [pushy-common](https://github.com/chef/pushy_common) Common code between the simulator and the service.

## Major Technologies used in Chef Push Server

* Erlang
* PostgreSQL
* ZeroMQ

If you're looking to contribute to certain parts of the push jobs service, familiarity with the
following related tools is also beneficial, depending on the area:

* rebar (used for dependency management in Erlang)
* sqitch (database migrations)
