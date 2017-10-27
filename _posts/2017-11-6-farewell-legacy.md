---
layout: post
title: Farewell
tags: [work, continuous delivery]
excerpt_separator: <!--more-->
---

This is it! (Michael Jackson), An unexpected journey (Peter Jackson) or Dark City (Alex Proyas). Those are show that would summarize my last years at Stratio. More than three years filled with soprt, passin, friend... that has reached its end.

<!--more-->

## My daily life

The last 3 years and 4 months, most of my work has been code-related. I started with a SQA role and went drifting to the DevOps one. Tons of intriguing technologies (Docker, Swarm, Weave, Ansible, Mesos, Jenkins), outputting a great outcome. I can't remember a day leaving the office and thinking my work was unproductive or without improvements. As of today, I have already forgotten the not so bright side.


## A legacy?

I suppose I will leave something positive. My main contributions have been focused on two efforts.

### BDT

An open source acceptance testing harness, used for each and every acceptance tests suites:

{% include image.html url="/images/bdt.png" desc="Stratio's acceptance testing harness trends" %}

It was me the one starting the project, almost from the shadows (without any request), and even it has receiver much more contributors, I feel it as a part of me:
{% include image.html url="/images/bdtme.png" desc="My contributions to the testing harness" %}

Most of my first year, I contributed to that project, just to easen my own real work: test automation. As the QA members sprout, the uses of the projects grew exponentially, managing to become (what I believe) the most used java library at Stratio.

This project strong keys would be:

* Reasonably well tested, with unit and integration tests (and tons of known issues).
* Offers a hyper-easy user interface (Cucumber).
* Allows integration with winner libraries beyond its scope (AspectJ).
* Multiple systems under test goals (MongoDB, Elasticsearch, Cassandra, Selenium, AHC).
* Extensible without limits, just implement Cucumber steps and sauce sith AssertJ checks.

### Continuous delivery [global shared library](https://jenkins.io/doc/book/pipeline/shared-libraries/#global-shared-libraries)

A closed source maven project, serving to more than 150 repositories (including the BDT one). It evolved from plain pipelines to multibranch ones. The repos being run from this library might be hosted both on GitHub or Bitbucket.

{% include image.html url="/images/cd.png" desc="Stratio's continuous delivery library trends" %}

Again, it was me the one starting the project, this time with a partial formal request (we want do continuously deliver software) and with a complete freedom to chose how, when and what to develop. This effort, even more that the BDT library, is a part of me:
{% include image.html url="/images/cdme.png" desc="My contributions to the continuous delivery library" %}

Up to three months ago, It was my precious, my pretty girl, the well to put all my care and interest in supporting others work. The more developments used it, the more it could bright. 
It contains unused features, such as [IPMI](https://en.wikipedia.org/wiki/Intelligent_Platform_Management_Interface) or [Marathon](https://plugins.jenkins.io/marathon) interactions, but also some others hugely embraced, such as ESX interactions.

For good or bad, it also became my biggest source of conflicts and nags.

This project is defined by:
* Having its own Jenkinsfile: Eats its own dogfood with a continuous delivery pipeline.
* This pipeline enables the project to become self distributable (via a docker image serving a git repo)
* Has _real_ unit tests, as described at [another post](https://www.linkedin.com/pulse/jenkins-global-shared-pipeline-libraries-real-unit-delgado-garrido/)
* Ruling over +150 different developments, it has suppor for a mixture of scenarios sucha as make, maven and gradle builds, sonatype automated gpg sign, deploy and publish (of course, just for FOSS developments, including the BDT one)

## The END

Yes. This is it!
