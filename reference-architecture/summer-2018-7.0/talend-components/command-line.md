---
title: "Commandline"
creationDate: "02/27/2018"
modifiedDate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Commandline

The CommandLine offers the same basic functionalities as Talend Studio and it is used to generate and export the Jobs developed with Talend Studio onto the Job servers, or export Services, Routes and data service Jobs onto Runtime servers. It is a Key component to enable Continuous Integration (CI) with Talend. In older versions of Talend CommandLine could be used to generate jobs on the Job Conductor or via Publisher (both in TAC). This is no longer recommended in favour of a binary deployment paradigm, utilising an Artifact repository.

The CommandLine can be executed in four different modes, according to your need:

- **Standalone/Basic mode** : This mode allows you to execute a single command.In this mode, CommandLine switches off after executing all commands passed on through the list of arguments. 

- **Shell**: In Shell mode, you can enter the CommandLine commands once and then only have to enter CommandLine's own keywords without having to restart CommandLine each time.

- **Server**: In Server mode, CommandLine can be accessed from the network for the purpose of executing commands. You do not have to wait the execution of a command to enter another one, you can enter several commands that will be executed in the same order you requested them.

- **Script**: In Script mode, CommandLine reads a script file containing a list of commands and executes them.

The most common mode used is the Server mode.

### Technical Details
- Server Component
- The CommandLine is an exact copy of the studio running in non-GUI mode
- Patches applied to the studio must also be applied to the CommandLine
- Can run as Service / Daemon 
- Require CommandLine on same server as Build Automation software (e.g. Jenkins) for CI

To understand more on Commandline please read <a href="https://help.talend.com/reader/RK~CAb9nJ1erxR8SrBbKoQ/w9WipT881wISUB7x1sPkAQ" target="_blank">Talend Help documentation</a> 

<!-- links -->
