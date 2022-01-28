# Slicing backlog items

## Stories, Themes, Epics

- choices of stories, themes, or epics bring an incredible amount of flexibility to a Scrum team
- understanding/usage dramatically improve the accuracy of their sprint planning sessions

- User Story
  - usually estimated using story points
  - self-contained unit of work
  - agreed upon by the developers and the stakeholders
  - building blocks of your sprint
  - "tool" used to create a conversation between the Dev Team and everyone else so the developers can estimate how much effort will be needed to deliver a specific outcome
  - a high-level description of a desired outcome/result
  - completed in one Sprint (generally), something actionable and small enough to fit in a sprint
  - should deliver a vertical slice of functionality to the customer that is valuable and complete by the end of an iteration
  - defined using INVEST criteria
  - Broken down into a series of Tasks
  - generally created by the customer or the product owner representing the customer
  - well-defined format/template: "As a `<role>` I want `<something>` so that `<value>`"
  - is a "What" that can fit in a single sprint
- Theme
  - groups of related stories
  - often the stories all contribute to a common goal or are related in some obvious way
  - However, while some stories in a theme may be dependent on one another, they do not need to encapsulate a specific workflow or be delivered together
  - example: [An example of a theme](https://www.jeremyjarrell.com/stories-versus-themes-versus-epics/)
  - is a cross-cutting concern that does not fit into a hierarchy of "Whats"
- Epic
  - T-shirt size or "it could take X to Y iterations to do this work"
  - resemble themes in the sense that they are made up of multiple stories
  - also resemble stories in the sense that, at first, many appear to simply be a "big story"
  - as opposed to a theme, however, these stories often comprise a complete workflow for a user
  - although the stories comprising an epic may be completed individually, they provide no measurable business value on their own
  - think of epics as a Story Arc
  - generally created by the customer or the product owner representing the customer (same as for User Stories)
  - is a "What" that transcends releases

- Themes vs. Epic
  - while the stories that comprise an epic may be completed independently, their business value isn’t realized until the entire epic is complete
  - it rarely makes sense to deliver an epic until all of the underlying stories are complete
  - while stories comprising a theme are related each is still independent enough to be delivered separately and still provide some measurable sense of business value

- Feature
  - chunk of functionality that delivers Business Value (revenue, engagement, etc.) that probably contains multiple User Stories and/or Themes
  - distinct element of functionality which can provide capabilities to the business
  - it generally takes many iterations to deliver a feature
  - a user story is a part of the feature
    - by splitting a feature in smaller stories, the user can give early feedback to the developers to issues quickly
  - is a "What" that can't fit in a sprint but can fit in a release

- Feature vs. Epic
  - the relationship between epics and features is the most controversial in the agile community
  - Stefano La Porta: an epic is a broader concept and an epic can be broken down into different features

- Task
  - estimated with hours or half days (in contrast to story points for User Stories)
  - are defined for each user story, so that the development team can have a clear sense of how it will accomplish its work
  - are a more granular versions of the work entailed to complete a user story
  - is a technical piece of work necessary to get a story done
  - developers split a story in technical tasks to get a realistic estimate of the time it will take to complete a story
  - decomposed parts of a story that get into HOW the story will be completed
  - usually defined by the people doing the work (developers, QA, etc)
  - is about the "How" and no one other than the team should be concerned with them
  
---

## Break down

- if User Story cannot get implemented because of dependencies, these dependencies need to get identified and resolved upfront
- maintain per user story a list of these dependencies (e.g. wireframes, UI, expert knowledge) which states also responsible person
- dependency removal costs time --> Grooming not to close to planning

if story cannot be estimated:

- Why does the story seem so difficult to estimate?
- Are the individual tasks that make up the story too complex?
- Does the story have dependencies on other work that has yet to be completed, or that must be completed by a third party?
- Are there technical or business unknowns in the story that are still unclear?

How deep to break down?

- break down further any story that is estimated above a certain threshold
  - starting point for this threshold: where your team has historically tended to become inaccurate with their estimates, e.g.:
    - team’s velocity tends to be relatively predictable when estimating stories of sizes 1, 2, or 3 points
    - but doesn’t have a great track record with stories sized at 5 points and above
    - then: any story estimated >= 5 points should automatically be broken down further before it's added to a sprint
- smaller stories travel the sprint board faster than a single larger  
  keep in mind: negative effect on a team’s moral as a single dominating story sets in the `In Progress` column for the majority of the sprint cannot be understated

### Sample to break down an Epic into Stories

first it seams to be a Story, but in reality more like an Epic: "As a salesperson, I’d like to set my password, so I can log into the system"

questions:

- How does the salesperson first access the system to set their password if their account isn’t fully setup?
- Do password strength requirements exist that will need to be enforced?

from Epic to Story:

- "As an Administrator, I’d like to send an email to a new salesperson containing a tokenized access link, so they may temporarily access the system in order to set their password."
- "As a Salesperson, I’d like to edit my profile, so I may set my password."
- "As an Administrator, I’d like to ensure that all salespeople’s passwords meet corporate strength requirements, so I can harden access to the system."

---

## Resources

- [Scrum Alliance, Jeremy Jarrell: Stories versus Themes versus Epics](https://www.jeremyjarrell.com/stories-versus-themes-versus-epics/)
- [Mike Cohn, Mountain Goat Software: User Stories, Epics and Themes](https://www.mountaingoatsoftware.com/blog/stories-epics-and-themes)
- [SE: What are the definitions and differences between: Theme, Epic, Feature, User Story and Task?](https://pm.stackexchange.com/questions/15000/what-are-the-definitions-and-differences-between-theme-epic-feature-user-sto)
- [SE: What is the weighting difference between Epic/Story/Task](https://pm.stackexchange.com/questions/16739/what-is-the-weighting-difference-between-epic-story-task)
- [SE: generally accepted hierarchy](https://pm.stackexchange.com/a/16784)
- [8 Tipps zum effektiven Einsatz von Scrum: Agile in der Praxis](https://entwickler.de/agile/8-tipps-zum-effektiven-einsatz-von-scrum-agile-in-der-praxis/)
