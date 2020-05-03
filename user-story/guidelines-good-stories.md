# Guidelines for Good Stories

## Start with Goal Stories

Consider each user role and identify the goals that user has for interacting with our software. 

For example, Job Seeker role -> Goal: find a job. This goal comprise the following goals:

* search for jobs she’s interested in (based on skill, salary, location, and so on)
* automate the search process so she doesn’t have to search manually each time
* make her resume available so that companies may search for her
* easily apply for any jobs she likes

These goals (which really are high-level stories themselves) can then be used to generate additional stories as needed.

## Slice the Cake

Large story, there are normally many ways of breaking it into smaller pieces. 

:x: Many developers is to split the story along technical lines.

> A far better approach is to write the replacement stories such that each provides some level of end–to–end functionality. Bill Wake (2003a) refers to this as "slicing the cake". 
 
* Exercising each layer of an application’s architecture reduces the risk of finding last minute problems in one of the layers.
  
* An application could conceivably be released for use with only partial functionality as long as the functionality that is included in the release slices all the way through the system.

**Example** "A Job Seeker can post a resume" like this:

* A Job Seeker can submit a resume that includes only basic information such as name, address, education history.
* A Job Seeker can submit a resume that includes all information an employer may want to see.

## Write Closed Stories

A **closed story** is one that finishes with the achievement of a meaningful goal and that allows the user to feel she has accomplished something.

**Example** "A recruiter can manage the ads she has placed" -> This is not a closed story

* A recruiter can review resumes from applicants to one of her ads.
* A recruiter can change the expiration date of an ad.
* A recruiter can delete an application that is not a good match for a job.

## Put Constraints on Cards

The practice of annotating a story card with "Constraint" for any story that must be obeyed rather than directly implemented. 

**Example** 

* The system must support peak usage of up to 50 concurrent users
* Do not make it hard to internationalize the software if needed later.
* The new system must use our existing order database.
* The software must run on all versions of Windows.
* The system will achieve uptime of 99.999%.
* The software will be easy to use.

Even better, acceptance tests can be written to ensure the constraint is not violated.

## Size the Story to the Horizon

Writing stories at different levels based on the implementation horizon of the stories. 

Stories for the next few iterations would be written at sizes that can be planned into those iterations, while more distant stories could be much larger and less precise. 

**Example**

* A Job Seeker can post a resume. 
  * A Job Seeker can add a new resume to the site.
  * A Job Seeker can edit a resume that is already on the site.
  * A Job Seeker can remove her resume from the site.
  * A Job Seeker can mark a resume as inactive.
  * A Job Seeker can mark a resume as hidden from certain employers.
  * A Job Seeker can see how many times her resume has been viewed.

## Keep the UI Out as Long as Possible

You want to keep the user interface out of your stories as long as possible. 

Eventually it will become inevitable for user interface details to slip into stories. This happens as the software becomes more and more complete, and stories shift away from being entirely new functionality to being modifications or extensions of existing functionality.

## Some Things Aren’t Stories

If you need to express some requirements in a form other than user stories, then do so.

If you find that some aspect of a system could benefit from expression in a different format, then use that format.

## Include User Roles in the Stories

If the project team has identified user roles, they should make use of them in writing the stories. 

Writing stories in this way keeps the user in the forefront of the developer’s mind. 

Each story can be written in the following format:

I as a (role) want (function) so that (business value)

## Write for One User

Stories are generally most readable when written for a single user.

## Write in Active Voice

User stories are easier to read and understand when written in active voice. 

**Example**

Rather than saying "A resume can be posted by a Job Seeker". 
Say "A Job Seeker can post a resume".

## Customer Writes

Ideally the customer writes the stories. On many projects the developers help out.

Additionally, because the customer is responsible for prioritizing the stories that will go into each iteration, it is vital that the customer understand each story. 

## Don’t Number Story Cards

Numbering story cards adds pointless overhead to the process and leads us into abstract discussions about features that need to be tangible.

## Don’t Forget the Purpose

Don’t forget that the main purpose of a story card is to act as a reminder to discuss the feature. Keep these reminders brief. 

Add the detail you need to remember where to resume a conversation, but do not replace the conversation by adding more detail to the story card.