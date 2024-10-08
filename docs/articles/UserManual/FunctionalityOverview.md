# Application Overview

Spira is an easy to use, quick to configure, application designed to work wherever you do (from big screens to tiny screens). It has powerful features to help you and your team collaborate to deliver high quality products to specification and on time. It is specifically focused on helping teams software and application development processes in a structured way.

This guide explains Spira's approach, what its different pieces are, how they fit together, and how you can use them together most effectively. This guide will explain the happy "good practice" paths to using it successfully. Most people work these ways and very successfully. Others take full use of Spira's flexibility and customization options to stretch the application to work outside the lines. These users are usually very successful too. The opening tip to this guide is this: where possible, work with the application not against it to have the greatest and easiest success.

This guide will hopefully be a useful learning resource, reference, and companion to the rest of the documentation. In particular, we recommend that brand new users, read this alongside the <a href="#">quick start guide</a>, which will give you practical hands-on steps to learn Spira.

!!! Tip "You say SpiraTest, I say SpiraPlan"

    The Spira family of applications comes in 3 different editions:

    - SpiraTest

    - SpiraTeam, which is SpiraTest plus some extra features

    - SpiraPlan, which takes all the features of SpiraTeam and adds a few more

    Where a feature is not available in all editions, you will see a little tag next to it showing the editions support. They look like this: <span class="pill">SpiraPlan</span>

## Core concepts

Spira's features are grouped together into different places that match up with different ways of using the tool.

!!! Tip "Tokens and IDs"

    Each item in Spira has a unique ID. This a globally unique number (1, 2, 3, and so on). Each type of item (a product, requirement, test case, etc) has a special two letter "token". Together with the ID this creates a shorthand unique reference to that item. Usually there is a colon between the token and the ID. For example, "RQ:7" represents the requirement with an ID of 7.

### Workspaces

Workspaces are the buckets where all the actual work lives.

The most common and important workspace is the product. This is where you and your team will spend most of their time. Products are long running areas of work with tangible outputs or goals. This can be a software or hardware product that gets new regular new releases, patches, and features. A product can also be used like a project, where the focus may be a different kind of output or to manage a process.

Each product lives inside a specific program. One program can have many products. Programs are where you group similar areas of work, outputs, or processes together. A program is more than a folder to store things. Programs give you insights into what is happening across all the products inside of it. Programs can also be used to track and manage higher-level goals than the ones in products.

<span class="pill">SpiraPlan</span> Programs live inside a **portfolio** . Portfolios can have many programs, and are another way to store and organize your work, and see insights about a collection of programs.

You can have as many products, programs, and portfolios as you need or want. Below is an example diagram showing how these different workspace related to each other.

```mermaid
graph TD
  ida(Product A)
  idb(Product B)
  idc(Product C)
  id1(Product 1)

  idd(Product D)
  ide(Product E)
  idf(Product F)
  id2(Product 2)

  id(Portfolio)

  ida --> id1;
  idb --> id1;
  idc --> id1;

  idd --> id2;
  ide --> id2;
  idf --> id2;

  id1 --> id;
  id2 --> id;
```


!!! info "Workspace glossary"

    | Workspace icon and name | Token |Description |
    | -------|------------|----------|
    | ![](https://spiradoc.inflectra.com/Spira-User-Manual/img/workspace-pr.png) &nbsp; Products | PR | Long running areas of work and deliverables
    | ![](https://spiradoc.inflectra.com/Spira-User-Manual/img/workspace-pg.png) &nbsp; Program | PG | Groups of products sharing similar overarching milestones
    | ![](https://spiradoc.inflectra.com/Spira-User-Manual/img/workspace-pf.png) &nbsp; Portflio | PF | Strategic collections of programs <span class="pill">SpiraPlan</span> |

### Artifacts

Artifacts are the building blocks of a product or program and contain all of their data. Each artifact holds different data and is used in different ways. For instance, requirements are one artifact, and releases are another. They work differently, and are not interchangeable. There are artifacts to help you test, plan, track bugs and tasks, and more.

You can use each artifact by itself and tag them in many different ways. An artifact can have sub types, a current status, priorities, components, owners, tags, and more. By linking one artifact to another, you unlock even more powerful features, letting you, for example, see which top priority user stories planned for the next sprint have failing tests still.



!!! info "Program artifact glossary"

    | Artifact icon and name | Token |Description |
    | -------|------------|----------|
    | ![](https://spiradoc.inflectra.com/Spira-User-Manual/img/artifact-cp.png) &nbsp; Capability | CP | Tracks program-scale features <span class="pill">SpiraPlan</span>
    | ![](https://spiradoc.inflectra.com/Spira-User-Manual/img/artifact-cp-parent.png) &nbsp; Capability (parent)	 | CP | Any capability that has one or more child capabilities <span class="pill">SpiraPlan</span> 
    | ![](https://spiradoc.inflectra.com/Spira-User-Manual/img/artifact-gm.png) &nbsp;  Program Milestone | GM | A way to group large scale deliverables together to hit a certain deadline <span class="pill">SpiraPlan</span> 

## Guidance and Tips
Below are explanations and guidance about how to do different things in Spira, or use its different features and artifacts (or links for where to read more). This includes good practice tips, tricks, do's and don'ts, and how different artifacts link to others. These are designed to help you get the most of out of Spira, and to help you work with the design of the tool, and not against it.

In each section you will see a short explanation of the feature or artifact. This is followed by a set of "**Tips and Tricks**". Most artifacts have a second tab to the right of "Tips and Tricks" that explains the "**Key Artifact Links**" you can make to others artifacts. The tab called "**Association Chart**" shows all the ways the artifact links to others

### Products

=== "Tips and Tricks"

    - Use all the artifacts that make sense for your needs
    - For every product try to always use requirements and releases
    - Link artifacts together to add meaning, improve tracking and    traceability, and give you and your team greater insights

=== "Association Chart"

    - Use all the artifacts that make sense for your needs
    - For every product try to always use requirements and releases
    - Link artifacts together to add meaning, improve tracking and    traceability, and give you and your team greater insights

### Users

Each person using Spira should have a dedicated user. A user by itself has no permissions or access to anything in the system. Administrators give them permissions in a few ways: to the user itself, adding them to a program, giving them a specific product role for a product (someone can be a manager with high level permissions in one product, but an observer with very limited permissions in another product). Artifacts can be linked to users, so you know who is leading on a piece of work. Users have a dedicated profile and personalized home pages.

=== "Tips and Tricks"

    - Limit who has roles with "bulk edit" permissions in each product
    - Severely limit who has system administrator permissions
    - Create dedicated users for any automation functions you use, like data syncs or unit testing. This will make it a lot easier to debug issues if they arise
    - Limit your use of the root admin account "administrator" and never use it for things like data syncs, to avoid the account being locked out

=== "Key Artifact Links"

    - Product Role: controls product membership and what permissions are allowed in each product
    - Program Role: controls program membership and what permissions are allowed in each program
    - Profile: personal information and settings for that user

=== "Associtaion Chart"

    - Product Role: controls product membership and what permissions are allowed in each product
    - Program Role: controls program membership and what permissions are allowed in each program
    - Profile: personal information and settings for that user

### Artifacts

See the links below to read specific information about each artifact.

- [Requirements](#)
- [Releases](#)
- [Test Cases](#)
- [Test Sets](#)

## Artifact overviews

=== "Test Automation"

    As well as being able to store and manage manual test cases, SpiraPlan® can be used to manage the scheduling and execution of automated test scripts for a variety of third-party test automation engines. This allows you to centrally plan your automated testing and monitor the results of automated unit, functional and load testing remotely. For example, you could schedule a set of automated functional tests to run on five different machines (each with a different browser/OS combination) at 2:00 AM and have the results be ready for the next morning

=== "Incidents"

    SpiraPlan® provides the ability to create, edit, assign, track, manage and close incidents that are raised during the testing of the software system under development. These incidents can be categorized into bugs, enhancements, issues, training items, limitations, change requests, and risks, and each type has its own specific workflow and business rules. Typically each incident is raised initially as a 'New' item of type 'Incident'. Following the review by the product manager and customer, they are changed to one of the other specific types, given a priority (critical, high, medium or low), and status changed to 'Open'. Once it is assigned to a developer for fixing, it is changed to status 'Assigned'.

    The developer now works to correct the incident, after which time its status changes to 'Fixed' or 'Not Reproducible' depending on the actions taken (or not taken). Finally the product manager and customer verify that it has indeed been fixed, and the status is changed to 'Closed'. SpiraPlan® provides robust sorting and filtering of all the incidents in the system, as well as the ability to view the incidents associated with particular test cases and test runs, enabling drill-down from the requirements coverage display, right through to the open incidents that are affecting the requirement in question.

=== "Tasks"

    As described above, in addition to storing the requirements for a product, SpiraPlan® includes the capability of drilling each lowest-level requirement down further into a series of work items called 'Tasks'. These tasks are the discrete activities that each member of the development team would need to carry out for the requirement to be fulfilled. Each task can be assigned to an individual user as well as associated with a particular release or sprint. The system can then be used by the product manager to track the completion of the different tasks to determine if the product is on schedule.

    The tasks can be organized into different folders as well as categorized by different types (development, testing, infrastructure, etc.), each of which can have its own workflow which defines the process by which the task changes status during the product lifecycle.

=== "Document Management"

    SpiraPlan® includes an integrated document management collaboration system that can be used to upload, manage and share documents between the different members of the product. This module includes support for uploading files and URLs, versioning of documents, the ability to organize into folders and categorize and search using meta-tags.

=== "Risk Management"

    SpiraPlan® (not available in SpiraTest or SpiraTeam) enables a complete risk management workflow. This module aids in the analyzing and categorizing of risks based on their Probability and their impact, which produces a calculated risk exposure. The tool tracks both risks and their mitigations, and provides dynamic risk reporting tools.

=== "Source Code"

    SpiraTeam® and SpiraPlan® let you browse your source code from within the main web application. This is an excellent way to browse all a product's code files, commits, and how a file changed in a commit (the 'diff'). There is no need to install version control software on your own computer or to clone the source code to your machine. All users can link source code commits with any SpiraPlan® artifact. This gives you traceability from requirements, incidents, tasks, and more to right code changes. This let you easily see what code was edited to implement a feature, or fix a bug. If the bug is reopened later, you can quickly see the associated source code commits to check if the changes made actually did fix things properly

=== "Build"

    SpiraPlan® integrates with a variety of continuous integration / automated build servers so that the results of automated builds can be displayed in SpiraPlan linked to the associated release or sprint. In addition, the results of automated tests and source code operations can be linked to the build events, providing traceability from a specific build to the bugs that were fixed, tests that were run, and source code files that were modified.

=== "Instant Messenger"

    SpiraPlan® comes with a build-in integrated instant messaging capability. This lets users see which users are currently logged-into the system, maintain a list of contacts and where available, send short instant messages to other users. Any messages exchanged can then be posted to relevant artifacts in the system as permanent comments.
