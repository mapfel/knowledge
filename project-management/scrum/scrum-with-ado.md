# Scrum with Azure DevOps

## Portfolio Management

- Portfolio backlogs provide product owners insight into the work done by several agile feature teams
- Product owners can define the high-level goals as Epics or Features
- Feature teams can break down these work items into the user stories they'll prioritize and develop

---

## Hierarchy of teams

- provide each feature team with their distinct backlog to plan, prioritize, and track their work
- portfolio or product owners can create their vision, roadmap, and goals for each release, monitor progress across their portfolio of projects, and manage risks and dependencies

### Sample

![ado.pm-team-structure.png](project-management/scrum/.media/ado.pm-team-structure.png)

- add a team for each feature team and management area
- move the area paths associated with feature teams from a flat structure to a [hierarchical structure](https://docs.microsoft.com/en-us/azure/devops/boards/plans/configure-hierarchical-teams?view=azure-devops#move-area-paths-into-a-hierarchical-structure)

  Flat area structure | Hierarchical area structure
  --------------------|----------------------------
  ![flat](project-management/scrum/.media/ado.team-list-hierarchy-structure.1.png) | ![hierarchical](project-management/scrum/.media/ado.team-list-hierarchy-structure.2.png)

  - open each area path associated with a feature team and change its location to be under the management area path
  - change the Location to move it under its corresponding management team area path

    ![ado.edit-area-path.png](project-management/scrum/.media/ado.edit-area-path.png)

- by including subarea paths for the management teams, you automatically include the backlog items of their feature teams onto the management team's backlog

  ![ado.include-sub-area-paths.png](project-management/scrum/.media/ado.include-sub-area-paths.png)

  ![ado.verify-area-path-assignments.png](project-management/scrum/.media/ado.verify-area-path-assignments.png)

- Management view of team progress, e.g. "Epics portfolio backlog for the Management team"
  - drilling down, you can see all the backlog items and features, even though they belong to one of three different teams: Customer Service, Phone, and Web

    ![ado.management-team-backlog-epics.png](project-management/scrum/.media/ado.management-team-backlog-epics.png)

- Assign work from a [common backlog](https://docs.microsoft.com/en-us/azure/devops/boards/plans/portfolio-management?view=azure-devops#assign-work-from-a-common-backlog)
  - while the hierarchical team and backlog structure works well to support autonomous teams to take ownership of their backlog, it also supports assigning work to teams from a common backlog
  - during a sprint or product planning meeting, product owners and development leads can review the backlog
  - teams can also assign select items to various teams by assigning them to the feature team Area Path

- [Teams without areas using a team field in TFS](https://nkdagility.com/blog/team-foundation-server-2012-teams-without-areas/)
  - if your organization has several teams that work from a common backlog and across many product areas, this configuration might not fit how you want to organize your work
  - by adding a custom field to represent teams in your organization, you can reconfigure the agile planning tools and pages to support your teams and decouple assignments into teams and area paths
  - when you customize your team project to support team fields, the Team field tab appears on the administration page for the team project, and each team

---

## Iteration and area path

- iteration Paths (aka sprints) support assignment of work items to time-box intervals
- defined at the project level
- each team selects the paths that they want to use
- are a shared resource used by all teams that select them
- You can create:
  - a flat set of iteration paths
  - a hierarchy of paths to support releases, sub-releases, and sprints
- while maintaining a single sprint cadence simplifies project administration, you can create different cadences as needed
  - for example, some teams may follow a monthly cadence while others follow a 3-week cadence
  - simply define a node under the top project node for each cadence, and then define the sprints under those nodes

- area paths allow you to group work items by team, product, or feature area
- you can review which Area Path(s) has/have been assigned to which teams

  ![ado.review-area-paths-teams.png](project-management/scrum/.media/ado.review-area-paths-teams.png)

- you can add area paths under the root area path
- each project typically specifies a predefined set of iteration paths to help you get started tracking your work; you only need to specify the dates

---

## Resources

- [MSDN: Use Azure Boards to manage your product and portfolio backlogs](https://docs.microsoft.com/en-us/azure/devops/boards/plans/portfolio-management?view=azure-devops)
- [MSDN: Configure a hierarchy of teams](https://docs.microsoft.com/en-us/azure/devops/boards/plans/configure-hierarchical-teams?view=azure-devops)
- [MSDN: Define iteration paths (sprints) and configure team iterations](https://docs.microsoft.com/en-us/azure/devops/organizations/settings/set-iteration-paths-sprints?view=azure-devops&tabs=browser)
- [MSDN: Team backlog iteration versus default iteration](https://docs.microsoft.com/en-us/azure/devops/organizations/settings/set-iteration-paths-sprints?view=azure-devops&tabs=browser#team-backlog-iteration-versus-default-iteration)
