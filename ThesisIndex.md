
Title:

Managing package drifts and guaranteeing system consistency in
distributed computing environments : using full-text-search engines and
continuous integration to ensure 

----

Abstract:

Thanks to the Agile approach, managing large number of machines has become
easier than ever: new technologies like Puppet allow service managers to
specify the server configurations in a text file and get it applied to the
machine in a timely manner. Moreover, since most of the virtual machines are
created using OpenStack, it's easy to replicate the configuration on multiple
servers or rebuild a broken machine in a completely automated way.



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
        * High number of machines

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
    
