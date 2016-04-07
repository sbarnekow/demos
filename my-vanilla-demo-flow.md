1. Introduction  
  1.1. Agenda
     - Demonstrating to show how easy GitHub makes it to socialize changes and solicit feedback
     - Build a better product, faster!
     - Implement, test, and deploy, painlessly. 
     - We will discuss: workflow and what a day in the life of a developer is like (when they're using GitHub)
  1.2 What is GitHub?
     - A set of features designed to allow software developers to work better together.
      - The world's largest host of open source code, used by over 12 million developers at work and home 
      - A place for code to be shared and reused across teams and organizations
    - Built on Git
      - Mature, stable, the most modern SCM framework.
    
  
2. Overview of demo environment  
  2.1. Today’s task
    - Make a change to a single page site running on GitHub Pages
  2.2. Describe the change we’re going to be implementing
    - Change default cities for the application
  2.3. Repository
    - HTML and Javascript project hosted on GitHub Enterprise
    - GitHub Pages is serving a static HTML website, changing this will allow us to illustrate the entire workflow
    1. GitHub is agnostic towards language, platform, deployment process.
  
3. Demo  
  3.5. GitHub at the center of SDLC
    - Lots of tools involved in your software development lifecycle
    - All code + discussion about that code lives in github
      - Canonical repositories
      - A single place to search in and deploy from
    - Integrates with best of breed software
    - Robust API that allows you to integrate with whatever you'd like
      - Specifically, an API for Status and Deployments combined allows you to deploy your code the minute it's merged into master

  3.4. Communication & Notifications
    - Use at-mentions to communicate with users and teams! 
    - Email notifications 
    - Web notifications
    - Team mentions which can also exist purely for the purpose of notifications
    - Collaboration! 
    1. Switch browsers
    2. See notifications
    3. Add line comment 
    4. Add PR comment
    
  3.2. GitHub Flow
    - Simple Git + GitHub workflow that allows teams to collaborate on changes that are isolated within a branch. The goal is to keep master in a deployable state at all times.
    - This can be done locally through your IDE. 
    1. Create a branch 
      - Branches are great because they are: super lightweight, quick to create, don't take up much disk space. Great way to isolate changes.
      - Edit a file and break the build so you can go into that later.
    2. Merge green PR and wait for deployment result. Go visit the updated site.

  3.1. Issue tracking
    - Issues are a great place to discuss changes to code before it's written 
    - A place where you can provide a framework for managing task
    - Includes an API for visualizing Issue data. 
    1. Create a new issue
    2. Apply a label for enhancement vs bug, or priority level
    3. Assign the issue to a developer
    
  3.3. Pull Requests
    - Pull requests are a great place to discuss and review changes to code as early as possible
    - Reevaluating an initial design or architectural decision gets more expensive as time goes on, sometimes it's too expensive to fix
    - Great place for people to share knowledge / experience 
    - Documents the decision-making process, brings it out of email, PRs are closed but never deleted, they're also searchable
    1. Open a PR 
    2. Reference the Issue created earlier, talk about the link between them.
    3. Include a detailed description, talk about Markdown! 
    4. Go into commits and line by line changes, dive into the details of what a PR is! Very exciting stuff.
    5. PRs can act as an agent for social change, PRs create a transparent development culture and help your developers write better code. Developers can learn from each others' mistakes and successes. Like Open Sourcing, you can Inner Source.
    6. Show a real PR
