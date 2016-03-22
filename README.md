# ioGlue

http://ioglue.io

[![Build Status](https://travis-ci.org/node-red/node-red.svg)](https://travis-ci.org/node-red/node-red)
[![Coverage Status](https://coveralls.io/repos/node-red/node-red/badge.svg?branch=master)](https://coveralls.io/r/node-red/node-red?branch=master)

A visual tool for orchestrating DevOps, based on node-red

![ioGlue: A visual tool for orchestrating DevOps](http://nodered.org/images/node-red-screenshot.png)

## Why
* Enable visual DevOps orchestration, or if you like - Node-Red for DevOps.
* In an Enterprise-grade, Cloud-Native way

## What
DevOps orchestration today involves multiple services, starting small but quickly growing large and complex, using spit-and-glue integrations, without any central system or tool for orchestrating everything.
The idea is to have ioGlue run as-a-service (either on-prem or on the cloud), and enable you to do in munutes what would otherwise take hours or days.
The idea is also to create a community around DevOps, to enable people and companies to share and collaborate around DevOps processes.

DevOps has enabled R&D and Operations teams to move forward very quickly. But what about the rest of the business? Right now, DevOps is 'stuck' in the 'server room'.

Once a DevOps is glued together using ioGlue, our vision is to enable connecting the rest of the business into DevOps, enabling effective and efficient communication and collaboration across the whole enterprise.

## How
Node-Red represents a new way of thinking, with regards to citizen integrations. It's not the first flow based programming tool, it's not the first citizen integration tool, but it is unique in the end user experience it provides. Simple and empowering.

DevOps, if you think about it abstractly, is just a bunch of services that emit events, and that can be triggered to do stuff, and some logic in between.

Input: web-hooks
Apply: business logic
Output: web-hooks

## No, really, how ?
* V1: MVP
 * Branch node-red
 * Strip out everything that's not necessary
 * Add Nodes for DevOps systems
* V2: Enterprise-grade (pull-request back to node-red)
 * Flow versioning & rollback
 * Audit log
 * Multi-user
 * Authorization & authentication
* V2: Cloud-Native
 * Add cloud native storageModules
   * Google Cloud Datastore
   * AWS *Something*
 * High availability / resiliency
   * ioGlue will be able to withstand any kind of failure without any side-effects to the users except for increased latency in execution of flows
   * Thinking: can we run ioGlue as lambda? that would be super cool, and also ultra economical.
   * State persistency ?
* V3: as-a-service

## Quick Start

Check out http://nodered.org/docs/getting-started/ for full instructions on getting
started.

1. `sudo npm install -g node-red`
2. `node-red`
3. Open <http://localhost:1880>

## Getting Help

More documentation can be found [here](http://nodered.org/docs).

For further help, or general discussion, please use the
[mailing list](https://groups.google.com/forum/#!forum/node-red).

## Developers

If you want to run the latest code from git, here's how to get started:

1. Install grunt, the build tool

        npm install -g grunt-cli

2. Clone the code:

        git clone https://github.com/node-red/node-red.git
        cd node-red

3. Install the node-red dependencies

        npm install

4. Build the code

        grunt build

5. Run

        node red.js

## Contributing

Before raising a pull-request, please read our
[contributing guide](https://github.com/node-red/node-red/blob/master/CONTRIBUTING.md).

## Authors

* Yaron Rosenbaum [@yaronr]

## Credits

Node-RED is a creation of [IBM Emerging Technology](http://ibm.com/blogs/et).

* Nick O'Leary [@knolleary](http://twitter.com/knolleary)
* Dave Conway-Jones [@ceejay](http://twitter.com/ceejay)

For more open-source projects from IBM, head over [here](http://ibm.github.io).

## Copyright and license

Copyright 2013, 2016 IBM Corp. under [the Apache 2.0 license](LICENSE).
