# Site Process Overview

## Document Summary
This is a living document. It is owned by the SITE team. Please feel free to make a PR with any additions, changes, subtractions, or ideas. 
We will discuss the PR as a team during stand-up and merge it if approved. 
Note: If the change is simply improved formatting, spelling, or grammar, please feel free to commit to the document directly without a PR.

We are lucky in that have minimal meetings and processes so that we can focus on our work and handle the realities of having a mostly part-time team.
Ahead is an outline of the minimal process and definitions intended to allow us to align as a team, focus, help our teammates, and guarantee the continued success of the project.

## Kanban
* This is a living board that we own which is, "designed to help visualize work, limit work-in-progress, and maximize efficiency" 
* Each individual and the team as a whole is responsible for ensuring its accuracy
* Please do your best to keep it up to date by creating tickets as needed and updating and moving them accordingly
* We base our Scrums and planning around the Kanban board and identify the following categories: 
    * TO DO, IN PROGRESS, IN REVIEW, READY FOR REVIEW, RESOLVED, and the BACKLOG
    * Note: All tickets in TO DO, IN PROGRESS, IN REVIEW, or READY FOR REVIEW, should be in (or placed in) the current release (or some future release, if the work spans multiple releases)

Definitions:
* TO DO
  * Work that needs to be done and/or analyzed
* IN PROGRESS
  * Tickets which are actively being worked on (e.g. analysis, development, etc.)
* READY FOR REVIEW
  * Tickets which have been completed, tested hyper-locally if applicable, and deployed to DEV if applicable.
* IN REVIEW
  * Tickets which are being actively tested, or otherwise reviewed
* READY FOR RELEASE
  * Tickets which have passed testing in DEV or their respective locations/forms and are ready for deployment to production (if applicable) for testing there (if applicable)
* RESOLVED
  * Tickets which have been deployed and have passed testing in production or are otherwise fully completed. 
  * Note: If a ticket should never have been created, please delete it. If a ticket was created but won't be completed, please resolve it but make sure to note the situation in the ticket. Also, please ensure there is no release attached to it.
* BACKLOG
  * Tickets that we need to complete but that are not yet part of a current release. If the ticket does not need to exist, please see the RESOLVED note.

## Jira Ticket Creation
* Create tickets whenever they need to be created. When in doubt, create it
* Add a Title using the following format
  * Project it includes, if applicable (if multiple projects then use commas to separate) followed by a colon, followed by a general description of the bug, problem, feature, or question. We don't mind different capitalizations or abbreviations or representations otherwise. Here are some examples:
    * RefVal: Review, install/run and merge external docker PR reference
    * site-ui: Remove C-CDA R1.1 Validator from UI (components and links)
    * Infrastructure: Update SSL certs as needed and install into Java
    * MDHT, RefVal: Integrate latest MDHT build into RefVal/add relevant JUnits
    * ETT GG: "google groups subject name"
  * If you are not sure of a project, do not let that keep you from creating the ticket. Simply create it, and add something/anything identifiable at that time, or later
* Add a description to the ticket. It must be formatted in a way where someone looking at it, who has no previous information, can work on it just as easily as the person creating the ticket can. However, that doesn't mean it has to be clear, analyzed, or complex, if that information doesn't exist yet. For example, if it's derived from an email, copying and pasting the email will suffice. If it's derived from a forum, copying and pasting the forum will suffice, along with a link to the forum thread. If there are files, attach them. As the ticket progresses and becomes more clear, feel free to update the description
* Move the ticket to TO DO and assign it to the current release if you think it can be completed within it and there are no other competing priorities. Otherwise, leave it in the backlog and place it where ever you feel it makes sense (top is highest priority, bottom is lowest)
* If you expect to be the one working on it, you can self-assign, or, if you know who will work on it, you can assign it to them. Otherwise, simply leave it unassigned
* If there is a question about priority, bring it up at the next Scrum or otherwise reach out

## Scrum
* Scrum is where we review the board, deal with blockers, address concerns, and delegate work. It is currently scheduled on Mondays and Thursdays at noon for a duration of 15 minutes. Please make your best effort to attend
* Due to the important decisions that must be made and planning that must be done, both the Scrum the day of the release and the Scrum before the day of the release are mandatory for all team members

## Planning
* Planning is where we decide what will be in the upcoming release and delegate work. It is a mandatory meeting which happens once a month after the prior release has been completed

## Release Preparation
* The release is scheduled for the last Monday of the month. If there is a holiday, it will be pushed to the following Tuesday
* One week before the release, before the Scrum, review whether or not a ticket will or can possibly be completed by the release it is tagged for. If it cannot be, remove the tag, or push it to the next release
* One week before the release, make a best attempt to have most or all tickets which are targeted for the release IN REVIEW. This is not a requirement, just a best-practice
* By the Scrum preceding the release day, all tickets which are targeted for the release must be READY FOR RELEASE (and pushed to dev), IN REVIEW, READY FOR RELEASE, OR RESOLVED. If this is not the case, and there are any tickets targeted for the release in TO DO or IN PROGRESS, the release will be pushed forward by one week
   * Note: It is possible to keep the release date in place if items can be moved accordingly or removed from the release during the Scrum. However, items which are removed will be pushed to the next official release. There will not be an extra release to accommodate them. This is why it may be preferred to delay in such cases as opposed to doing a smaller release
* By the Scrum preceding the release day, if possible, make a best attempt to create and add release notes to the ReleaseNotes.md file located at https://github.com/onc-healthit/site-content/
  * If there is only a master branch, create a new branch with the version of the release that is about to happen as the name, and update on that branch. If there is already a version branch for release that is about to happen, add updates to that branch
        * Release notes should be written in present-tense. See the Release Notes section for more information

## Release Day Process
* If not already done, release notes must be created and added to https://github.com/onc-healthit/site-content/blob/master/ReleaseNotes.md, __before__ the release day Scrum so that the team can review them on the call
* Ensure all tickets for the release are in their proper (current) location by 5pm eastern at the absolute latest
* Identify what you will be handling for the release and present this at Scrum so that a plan for the release and team member's actions can be formed. This can likely be easily derived from the release notes
* Find out if there is anything you can help out with otherwise in regards to deployment, github releases, site-content, etc.
* A typical release is targeted to start at 9pm. If there are issues in deployment of the release which are not resolved by 11pm, the release will be delayed by at least one day. 
   * Note: As stated earlier, if the reason for the delay is related to items not being in dev by the Scrum preceding the release day, then the release would have already been pushed forward by one week, and we wouldn't be attempting a release at all

## Retrospective
* This is where we review what was done well and what could be improved in regards to the finished release. It is a mandatory meeting which happens once a month after the current release has been completed

## Commits
* Commits should be written in present-tense. This imperative-style comes from the git documentation and makes the commits shorter. Is it the best way to do things? Maybe, maybe not. But, it will align us, and that is more important than the choice. To help with this, think of using words like the following to start your commit messages: Fix, Add, Remove, Change, Update, etc. Basically though, describe what you are doing at that moment/or commanding of the codebase, not what has been done to it. For example:
  * Update API Content URL on Scorecard Batch Application
  * Fix ActStatus Value Set OID
  * Add support for IVL_REAL data type and implementation on organizer
  * Limit Vital Sign Observation/value to data type PQ
  * Require provenance identification using templateId for provenance TS validation
        * Note: This is from Git documentation: "Describe your changes in imperative mood, e.g. "make xyzzy do frotz" instead of "[This patch] makes xyzzy do frotz" or "[I] changed xyzzy to do frotz", as if you are giving orders to the codebase to change its behavior."
  * If you would like to add a further, detailed description, in past-tense, it is suggested to add a new line which begins with a hyphen and to type it there. However, this part of the formatting is up to you and is merely a suggestion
* Commits should be able to be used as a release note fairly easily

## Release Notes 
* Release notes should be written in present-tense. They should be able to be derived from a commit fairly easily, or a series of commits with little effort

## Documentation
* If for any reason a team member finds that they could help others in the future through documentation, please create it and place it here:
  * https://oncprojectracking.healthit.gov/wiki/collector/pages.action?key=SD
* Currently there exists documentation for infrastructure updates (e.g. Java, Artifactory, Postgresql, Tomcat, DNS) as well as testing and usage of some of our services/applications. This will be of immense help to other team members and future team members as well as the client and reduce repetition and training time

## GitHub Releases
* TO DO

---

# Approval list
* [X] Dan    | PR for update [No]
* [] Sandeep | PR for update [?]
* [] Brian   | PR for update [?]
* [] Mounika | PR for update [?]
* [] Girish  | PR for update [?]
* [] Prabhu  | PR for update [?]
* [] Sean    | PR for update [?]
* [] Dragon  | PR for update [?]
