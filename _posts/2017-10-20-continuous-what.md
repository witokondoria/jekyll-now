---
layout: post
title: Continuous what?
tags: [continuous integration, continuous testing, continuous delivery, continuous deployment]
excerpt_separator: <!--more-->
---

How awesome is to perform duties in an automated way! And something running in an automated fashion could be kept rolling on forever. And this forever implies the word continuous.  

Understanding continuous X (being X some variable concepts such as integration, testing, delivery or deployment) is not that difficult. The real hiccup comes with implementations and speed bumps, setup by us, persons.

<!--more-->

## What's the deal?

For understanding continuous X, this Puppet blog image summarizes the global idea:

![_config.yml](https://puppet.com/sites/default/files/2016-09/puppet_continuous_diagram.gif){: .center-image }

It comprises several stages, run within a linking pipeline, where some of them might be automatic and some others might require a human intervention (hence, the _subtle_ difference among delivery and deployment). 

Add to that image some fine information:

 * Some of these stages could/might/should be run in parallel.
 * Some others might fail without braking the whole pipeline.
 * There could even exist retries to avoid stages failing, so loops could happen

And thats all folks! You just need some _real_ work to develop software that performs it. Sauce it on over your favourite tool (hint: [https://jenkins.io](jenkins)), stir it well (hint: [https://jenkins.io/doc/book/pipeline/io](pipelines)) and let the magic flow.

## Then, where is the problem?

Already said: humans. We trend to make things difficult, behave in distinct ways on distinct days. Anyone willing so could forge a system for performing your chosen X (integration, testing, delivery, deployment ...).  

From my experience, these are the real stoppers:
 * The system becomes underused to the point that no deployment is performed.
 * No further development - bugfixing is done to your awesome develpment.
 * There are no investments in order to improve the underlying infrastructure reliability (HA anyone?).
 * There are no investments in order to properly monitor the system, so fallouts could happen without warnings nor room for maneuver.
 * The competencies related to the system mainteinance become blurry: no one takes care of it, but it must be taken care of (notice the incongruence)
 
 In any case, we will be shooting the very core of the system, with possible terrific consequences.
 
## So?

Run away from such situations and __always__ pamper your work and related elements. You will be sowing to harvest.
