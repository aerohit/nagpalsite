---
layout: default
title: Resume
---

# The technical details
-----------------

## Overview of my current and previous jobs

### Research Engineer at **INRIA**, France (Jan 2013 - present)

I am currently working as a research engineer at **[INRIA](http://www.inria.fr/en/)** with the
**[KerData](http://www.irisa.fr/kerdata/doku.php)** research group, which is focussed on development
of Scalable Storage for Clouds. I am hired to develop features in [BlobSeer-WAN](http://blobseer.gforge.inria.fr/doku.php),
a large-scale data storage service on geographically distributed clusters. My work here includes:

- Implementing asynchronous replication of data saved on one site to other geographically distributed sites to 
  facilitate faster access. 

- Using BlobSeer-WAN as a more efficient storage backend for HGMDS, a distributed metadata management
  system for global file systems, and study the performance gains.

I am getting experience in developing storage for big-data in the order of terabytes supporting high throughput
under heavy concurrent access. The storage service is written in C++ and makes heavy usage of Boost libraries.

### Software Engineer at **iLodge** (Jul 2011 - Dec 2012)
**[iLodge](http://www.ilodge.com)** is a start-up in travel space, trying to develop a 
cloud based enterprise platform called *Connect* to combine tech and non-tech components for 
online travel; bringing in travel and social media closer. I was the third employee and
a core member of a team comprising of people from Google and Adobe. Some of the work that I have done 
here includes:

- Indexing framework over [Amazon SimpleDb](http://aws.amazon.com/simpledb/) to provide search over
  the data maintained by iLodge. Also implemented *hierarchical* indexing for range-type attributes. 
  SimpleDb puts a restriction on the maximum number of values for any attribute while searching. There
  are some range-type attributes which can be indexed hierarchically. The hierarchical index circumvents
  these restrictions and allows larger searches.

- A fault tolerant background task framework for executing tasks in a non-blocking, 
  retryable manner. In a cloud based application tasks could fail due to unavailability
  of servers and hence they should be retryable. This is used extensively by the indexing 
  framework and other services. Tasks which have failed are automatically triggered 
  whenever the corresponding server is up.

- Transaction framework for executing transactional database operations. SimpleDb is not a relational
  database and it doesn't provide complex transactions and relations. Hence this framework was
  developed to provide support for complex operations.

- An id-generator to generate unique string-ids for data to be persisted on *Amazon SimpleDb*. 
  SimpleDb is a non-relational database, and unique reference to the data has to be generated.
  The challenge is to ensure uniqueness across multiple instances of JVMs or application
  servers running in parallel and their corresponding shutdown and restarts.

- An automatic code generator for generating [GWT](https://developers.google.com/web-toolkit/)
  json overlays by parsing [protobuf](http://code.google.com/p/protobuf/) files. These json overlays
  are JavaScript equivalent of [POJOs](http://en.wikipedia.org/wiki/Plain_Old_Java_Object) and are
  used extensively on the browser UI to handle client side data. Their automatic generation 
  saves considerable amount of developer time.

- A *time profiling* tool for measuring the performance of the cloud based multi-threaded
  application. This tool helps to analyze and subsequently optimize the time taken to execute any 
  operation including that by individual threads started by its execution.

- A *[generic](http://en.wikipedia.org/wiki/Generics_in_Java)* REST api for the various
  entities/resources persisted in the database.

- A framework for management of inventories of products being sold by *Connect*. 

While working here I have learnt about designing and implementing a cloud based, distributed
platform based on services-oriented architecture from scratch.


### Research and Development Engineer at **Knowlarity** (Apr 2011 - Jun 2011)
**[Knowlarity](http://www.knowlarity.com)** is a mid-sized company in the domain of *cloud
telephony*. I was working in their core technical team to develop a scalable platform to 
create and host their products. My work here included:

- Developing an innovative *IVR* based trouble shooting system to be used by power plants. This
  system was a very cheap alternative to sophisticated/costly trouble shooting systems used
  by technicians in difficult locations.

- An information gathering and dissemination system used by the government of Uttar Pradesh
  for collecting daily statistics related to mid-day meal scheme run in primary schools.

- Developed a notification system to report failures in performing requests by the services 
  underlying their platform and persisting information to debug and/or execute them again.


### Application Developer at **ThoughtWorks** (Jun 2010 - Mar 2011)
**[ThoughtWorks](http://www.thoughtworks.com)** is famous as one of the pioneers of Agile
software development.

- Worked on a project to setup an internal cloud for ThoughtWorks using [OpenStack's](http://openstack.com) 
  cloud controller to create Virtual Machines on the fly for their development teams. My task
  included deploying it on a yet untested distro (CentOS), submitting bug fixes, writing bash
  scripts for automatic deployments of missing dependencies etc.

- I also developed database backed enterprise web applications in Ruby on Rails framework.

- Learned best practices of software development including Test Driven Development,
  Design Patterns, DRY principle, etc from the best in the industry.
