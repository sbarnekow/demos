# Vanilla GitHub Enterprise Demo

## Purpose of this document

* This document contains a general structure and a number of talking points which can be used as the skeleton for a vanilla demo.
* This document is not a script. It should be used to build a demo plan which is specific to the customer's use case.
* SE's should be comfortable running through and talking about all the points described below.
* This is a living document that should be updated often by all members of the team.

## General Guidelines

### Narrative

The general narrative we use when talking to customers is described below. The demo should be used as an opportunity to drive these points home. Ensure that you understand why these points are important to customers.

* GitHub helps reduce the complexity of building software.
* GitHub allows your developers to work collaboratively.
	* Collaboration increases productivity, quality and innovation within a software development team. More eyes, ideas and experience looking at every problem.
* GitHub allows your developers to work in the way that makes them most productive – big ecosystem / sync vs async
* GitHub encourages reuse & sharing of code & knowledge. Inner sourcing
* GitHub leads to happier and more productive developers. Retention and attraction.

### Preparation

* Follow the [demo prep guide](../onboarding/preparing-to-demo.md) to get your hardware and software set up
* Every customer has a pain point — that’s why they are talking to us. Make sure the sales rep has clearly articulated to you what the customer’s pain point is. If they don’t know, they have to go back and find out.
* Know how you are going to address the pain points. The customer should leave the demo feeling that GitHub will solve their problems.
* While we don’t necessarily go into a technical deep dive of Git, be prepared to do so. It’s is still something we need to have an advanced understanding of.
* Remember to tell the customer what you're going to show them before you show them. Follow up with the reasons why they should care.
* Know your audience. Do your research before hand.
* Gain as much context as possible. Understand the customer's industry, their competitve threats and their software needs. Have the sales rep help you.
* Practise your demo
* Double check that everything is working

### Jargon

* Think about the words you use. Watch old demos and make a note of the jargon you use.
* Make sure you define all Git terminology before using it - this includes clone, branch, master, repository, push, pull, rebase, etc.
	* The words you use may have a different meaning in another VCS. Be sure to clearly describe what it means in the context of Git
* GitHub jargon includes Pull Requests, Issues, Markdown, @mentions, Status API, Atom, Desktop, Stafftools, Webhooks, etc.

### Demo content

* Aim to make the demo as real as possible. The repo, conversation, changes and deployments we have should all look like they are part of a real project.
* Unless otherwise stated, stick to showing GitHub Flow instead of focussing on Git itself.
* Tailor the content based on the customer's requirements. Capture the tailored content for the rest of the team.
* Where possible, use bots and the API to give the sense that people are actively involved in the conversations you create during the demo.

## Content

1. Introduction  
  1.1. Agenda
    * What we’re going to show in the demo
      * A day in the life of a developer using GitHub
      * A workflow for discussing, implementing, testing and deploying a single change
    * Why we’re going to show it
      * Show how easy GitHub makes it to socialize changes and solicit feedback
      * Build a better product, faster
      * Implementing, testing and deploying changes should be a painless process
    * What we’re not going to focus on in the demo
      * Git commands
        * Important but focus is on GitHub workflows
      * Working in our local IDE - do all the same things but through the browser

  1.2 What is GitHub?
    * Set of features designed to allow software developers to work better together
      * Where teams come together to discuss and review changes to  code
      * Place for code to be shared and reused across team and organization
      * World’s largest host of open source code
      * Used by over 10m developers at work and at home
    * Built on Git
      * Mature
      * Stable
      * The tool the majority of professional software developers prefer

2. Overview of demo environment  
    2.1. Today’s task
      * Make change to a single page site running on GitHub Pages
      * Website allows you to find a meeting time between 2 or more cities

    2.2. Describe the change we’re going to be implementing
	  * For example: The default cities used by the site aren't applicable to the majority of users. We're going to change them to ones which are
      *  Reported to us by a user via email

    2.3. Repository
      * We have an HTML & Javascript project on GitHub Enterprise
      * Using GitHub Pages we host a static HTML website
        * Allows us to easily illustrate the entire workflow.
        * GitHub is agnostic towards language, platform, deployment process

3. Demo  
  3.1. Issue tracking
    * What and Why?
      * Place to discuss changes to code before any code is written
      * Provide a framework for managing tasks - labels & milestones are flexible.
      * Strong API for reporting & visualizing data
    * Log the issue based on 2.2 above
    * Apply a label - is it an enhancement or bug? Is it a high priority?
    * Assign it to a developer

  3.2. GitHub Flow
    * What and Why?
      * A simple Git & GitHub workflow
      * Allows teams to easily collaborate on a change that is isolated in a branch
      * Master is always in a deployable state
    * Reiterate that this can be done locally through almost all IDEs
    * Create a branch
      * Explain what a branch is:
        * Way to isolate changes
        * Quick to create & doesn’t take up much disk space
      * Edit a file to implement the change described in 2.2
        * If possible, break the build so that there is something to discuss in 3.5. There is a spec that will fail if the default cities are changed. Feel free to add specs to cover whichever scenario you describe in 2.2. Guidelines on how to write Jasmine Specs are available at http://jasmine.github.io/2.2/introduction.html.

  3.3. Pull Requests
    * What and Why?
      * Allow you to discuss and review changes to code as early as possible
        * Reevaluating an initial design or architectural decision gets more expensive as time goes on. Sometimes too expensive to fix.  
      * Provides a place for people to share knowledge and experience
      * Documents decisions made during the development and review process
        * No longer hidden in email
        * PRs can be closed but never deleted
        * PRs are searchable so previous discussions on a topic can be quickly found
        * Makes it easier to onboard new team members
    * Open a PR
      * Try not to spend too much time typing unless you can talk while doing it
        * Have the content prepared and available to copy and paste (consider using a text expander)
      * Title of the PR should start with an action
      * Reference the Issue you created in 3.1
      * Include detailed description of the change & task list
        * Use this as an opportunity to talk about Markdown
          * Markup language with plaintext formatting syntax
          * Easy to read, easy to write
          * Converted to HTML by GitHub
    * Describe components of a PR (which allow you to review changes at all levels)
      * High level conversations - opportunity to talk about architecture and design
      * Commits
      * Line by line changes - opportunity to dive into the details
    * Agent for social change
      * Pull Requests create an transparent development culture
          * Encourages adherence to best coding practices  
      * Developers can learn from each others' mistakes and successes
    * Show a real PR -- atom/atom has great ones (e.g. #2507)

  3.4.  Communication & notifications
    * What and Why?
        * There is a lot of conversation happening on GitHub at the same time
            *  It's difficult and unnecessary to follow every conversation
        * At-mentions allow you to bring the right people into the conversation at the right time
        * Everyone can focus on what's most important to them while still being accessible
    * @mentions allow you to notify users or teams about something happening on GitHub
        * Email notifications allow for asynchronous communication
        * Web notifications for synchronous communication
        * Team mentions
            * Teams on GitHub exist to manage access to repositories
  	        * Users can belong to multiple teams and teams are granted specific access to a set of repositories
    	* Teams can also be purely for notifications.
      	  * Let people self-select based on passion & interest
      	  * Doesn't have to map to organizational structure
    * Collaboration — switch browsers, see notification, add line comment, add PR comment

  3.5. GitHub at the center of SDLC
    * What and Why?
        * Lots of different tools involved in the process
        * All code and discussion around code lives on GitHub.
	        * Canonical repositories
	        * Single place to search
	        * Single place to deploy from
        * Integrate with other tools using our API and pipe information back in
        * Single way of displaying information regardless of the tools being used

    * Build Status
        * Using the API we’ve notified the CI server that there’s a change that needs to be tested
        * Without leaving the page, everyone involved in the PR can see the build is failing

    * Deployments
  	* The Deployments API allows you to start the deployment process.
        * Combined with the Status API, you’ll be able to coordinate your deployments the moment your code lands on master.
        * Merge green PR and wait for deployment result. Go visit the updated site.

## Choose your own adventure

1. Customizing the demo repository [replaces Section 2]
	* Once you're comfortable with this vanilla demo, feel free to customize the demo repository to fit your style
	*  Choose a relatable language/framework -- seeing a bunch of Closure probably isn't something our customers are used to
    * Solve a real problem in the demo process
    * Set up CI and CD
    * Prepare Issue and PR content relevant to the story you are telling prior to the demo

2. Fork & Pull [added to Content 3.2]
    * What & Why?
        * Process used by some of the largest OSS projects
        * Allows you to gate merges
            * Only a core group of project maintainers can merge Pull Requests
        * Doesn't stop people with read access from proposing a change
        * If you don't have write access to a repository, you can fork it
            * Creates a sandboxed copy of the repository within your personal account
            * Allows you to make changes to the fork but not the canonical repository
    * Switch to a user with only read access
    * Fork the repository into your account (make sure you delete an existing fork prior to the demo)
    * Create a branch, make a change and submit a PR [follow process in Content 3.3]
    * Point out that the Pull Request lives on the upstream repository
    * Point out that the Pull Request cannot be merged by the user with read-only access

3. Setting up a custom web hook [added to Content 3.5]
    *  What and Why?
        * There are a number of internal, legacy or niche tools which you may want to integrate with GitHub
        * Web hooks and the API make it easy to build middleware to support these integrations
            * Easy to use authentication system - OAuth & Application Tokens
            * RESTful API with great documentation & an active community
        * Web hooks POST JSON data to a given URL when certain events occur on GitHub
                * JSON data has all the information you need   
                * Push based systems
    * Create a new [requestb.in](http://requestb.in/)
    * Use the requestb.in URL to create a new web hook
    * Choose the specific events you want to subscribe to
    * Kick off the even (open or comment on an Issue)
    * Reload the requestb.in to show that it has received the payload
        * Show how easy it is to parse the data and react to it

4. Tag & Release
    * What & Why?
        * GitHub Releases are a way of shipping software to end users
        * Allow you to attach change logs and binary assets
        * Linked to Git tags - history of the project provides context for the release
        * API allows you to create releases automatically

5. Complex branching models
    * This is a time consuming topic and requires at least a foundational understanding of Git. Refrain from including this in the first demo.
    * For projects with long living releases, show Git Flow
        * Master has tags indicating the version of the production release
        * Develop is in a good state and the one people branch off
        * Work is done in feature/topic branches
        * Hotfix branches are used to patch production releases

6. Documentation
	* What and Why?
        * Documentation is most useful when it lives close to the code -- less context switching
        * Traditionally, it's difficult to keep documentation up to date
        * GitHub provides 3 different ways to manage your documentation. All are easy to use, versioned and beautifully rendered
    * GitHub allows you to produce internal documentation
	    * Style guides, project structure, security guidelines, etc.or
    * GitHub allows you to produce external documentation
	   * User docs, api docs, license info and contributing guidelines
	* Wikis
        * Each repository has a built in wiki
        * Git backed
        * Simple and easy to use
    * Markdown files
        * Markdown is a plaintext markup language which GitHub understands
        * Text files with .md extension are rendered -- files themselves as well as diffs
        * Lives next to your code in the Git repository  
             * Pull Requests which change code should also change documentation
	* GitHub Pages
        * Create project specific websites
        * Code lives on a separate branch within the Git repository
        * Built in templates allow you to quickly create a site to market a project internally

7. Reporting
    * What and Why?
        *  Project managers and team leads need a higher level view of what is happening on GitHub
     * Pulse (demo using atom/atom)
         * Get a overview of what has been happening on a repository over a certain period of time.
         * Great for catching up on a repository that you're not actively watching
      * Repository Graphs (demo using atom/atom)
          * Contributions graph shows who has been adding or removing lines of code from a project over a period of time
          * Adding code is easier than removing it. Looking at who has deleted the most number of lines will give you a sense of who knows the code base best
          * Network graph will show all forks and their state relative to the upstream repository
      * Almost all data that is available in the web UI is available through the API -- easy to build your own reports
          * http://issuestats.com/  

8. Admin console walkthrough
    * A full tour of the admin console is generally a topic for a separate demo
    * For a quick overview, go through the following:
        * Monitoring and settings pages in the management console.
        * Instance activity graphs and audit logs (/explore)
        * Stafftools - adjust force push settings on an organization
    * Show github/backup-utils and explain HA configuration

9. JIRA integration [updates Section 3.1]
10. Using a bot to give a sense of collaboration
