---
title: Application Orchestration for Cloud Foundry : Part 2
layout: post
---
<link rel='stylesheet' href='../css/markdown7.css'/>
## Application Orchestration for Cloud Foundry : Part 2 

[TOSCA](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) is an open standard for describing and managing portable cloud applications. Version 1.0 of the specification defines a YAML syntax to describe **both** the topology and behavior of cloud applications.

> In this section, we will focus on describing the application topology. Later, we will show how to leverage TOSCA to add orchestration and management behavior to this topology. 

1. [Deploying an application on two clouds](2015-05-07-multiple-cloud-foundries.html)
1. [Describing with a TOSCA blueprint](#l1)
1. [Scaling with a local workflow](2015-05-07-workflow-for-cloud-foundries.html)
1. Orchestrating with a Cloudify plugin
1. Collecting logs and metrics

## <a name="l1"></a>Describing with a TOSCA blueprint

YAML is well-suited to the task of describing our still-somewhat-simple application. 

### Application Topology

### Deploying the Blueprint

### Result

![Many providers](images/many.png)

Next, we will use TOSCA to map a local workflow which enables us to scale the application up and down across PaaS providers.

[< Last](2015-05-07-multiple-cloud-foundries.html) | [Next >](2015-05-07-workflow-for-cloud-foundries.html)