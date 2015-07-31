
Title:

Managing package drifts and guaranteeing system consistency in
distributed computing environments : using full-text search engines and
continuous integration to ensure servers configuration.

----

Abstract:

Thanks to the Agile methodology, managing a large number of machines has become
easier than ever: new technologies like Puppet allow service managers to
specify the server configuration in code and get it applied to the
machine in a timely manner. Moreover, since most of the virtual machines are
created using OpenStack, it is easy to create machines on the fly and use
Puppet to configure them in a completely automated way.

The downside of this approach is that the service manager doesn't know
exactly how machines are configured and relies on the software to keep all the
configuration aligned and syncronized. Any intervention, package upgrade and
software configuration is managed by the configuration management utility.

At CERN the number of servers has grown dramatically in the last years and this
leaded to a situation quite common in big datacenters and usually difficult
to address: configuration and package drifting. In fact, every time an upgrade
is released, it is not easy to detect if all the machines updated their
configuration correctly and why a misconfiguration happened.

This thesis analyses the causes of the problem, trying to address it using
a set of open-source softwares like ElasticSearch and Jenkins in combination
with the development of a custom solution called "Package Inventory".

----

Index:

* Aim of the thesis

* Introduction
    * Agile Methodologies
        * Continuous development
        * Continuous delivery
        * Continuous integration
    * Infrastructure Drifts
        * Package Drifts
        * Configuration Drifts

* Computing at CERN
    * Datacenters
    * Cloud Computing
        * OpenStack
    * Monitoring
        * ElasticSearch
        * Kibana
        * Flume
    * Configuration Management
        * Puppet
        * Foreman
        * Git
        * Jenkins
        * Koji
        * Jens
        * Rundeck
        * Mcollective
        * Roger
        * TBag

* Configuration Management
    * Current Infrastructure
    * Module, Hostgroups and Environments
    * Puppet Run
    * Configuration Change process
    * Problems
        * Multiple service managers
        * Deployment interval
        * Configuration and package drifts

* Package Inventory
    * Project description
    * Metric structure
    * Store metrics with ElasticSearch
    * Reporter
        * Yum
        * RpmDb
        * Functions
        * Report changes with Flume
    * Cli
        * Functions
        * Querying ElasticSearch
        * Optimizations for large-scale queries
    * Packaging with Koji
    * Deployment
    * Results
        * Deployment size
        * Performance Analysis

* Continuous Integration with Jenkins
    * Aim of the project
    * Current status and problems
    * Workflows re-engineering
    * Customizable testing
        * Machine manifests
        * Module dependency
        * Internal/External machine testing
        * Testing mode (Rebuild/Env change)

* Conclusions
    * Current Status
    * Performance Report
    * Future plans
        * Package Inventory
        * Continuous Integration

