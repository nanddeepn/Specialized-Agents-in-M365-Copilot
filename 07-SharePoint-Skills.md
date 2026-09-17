# Lab 7 -- SharePoint Skills

## Introduction

Skills extend Copilot in SharePoint with reusable instructions for
repeatable work. A skill can package a multi-step workflow so users do
not need to rewrite the same detailed prompt every time.

Microsoft stores SharePoint skills as Markdown files in the site's
**Agent Assets** library under a structure similar to:

`/Agent Assets/Skills/<skill-name>/SKILL.md`

Skills use capabilities already available to Copilot in SharePoint. They
do not grant extra permissions, execute arbitrary custom code, or
independently connect to external systems.

## Prerequisites

Microsoft currently documents:

-   Access to a SharePoint site where Copilot in SharePoint is
    available.
-   **Edit** permission to create skills.
-   **View** permission to use skills.
-   Appropriate permission to any SharePoint content the skill works
    with.

## Exercise scenario

Create a reusable skill that reviews project status documents and
produces a consistent weekly project summary.

## Exercise 1 -- Discover skills

1.  Open Copilot in SharePoint on the workshop site.
2.  Enter:

`/skills`

3.  Review the built-in skills available in your environment.

Discuss the difference between built-in capabilities and custom reusable
skills.

## Exercise 2 -- Create a skill

Ask:

> Create a skill called Weekly Project Review. When I run it, review the
> project status content available in this SharePoint site and produce:
> Overall Status, Progress This Week, Upcoming Milestones, Risks,
> Issues, Decisions Needed, and Actions. Do not invent owners or dates.
> Flag missing information. Keep the final output suitable for a project
> steering meeting.

4.  Review the generated skill definition.
5.  Ask Copilot to refine any unclear steps.
6.  Save the skill.

## Exercise 3 -- Run the skill

Ask:

> Run the Weekly Project Review skill.

Check whether the output follows the same structure you specified.

Then add or update a workshop project document and run the skill again.

## Exercise 4 -- Make the skill parameterized

Ask Copilot to improve the skill:

> Update the skill so I can specify the reporting period and optionally
> a project name. If no reporting period is provided, ask me for it
> before generating the report.

Run it again with:

> Run Weekly Project Review for Project Falcon for the week ending 18
> September 2026.

## Exercise 5 -- Inspect the skill file

If permitted:

1.  Open **Site contents**.
2.  Locate **Agent Assets**.
3.  Browse to the Skills folder.
4.  Locate the skill's `SKILL.md`.
5.  Review the instructions.

Avoid breaking the expected file structure when manually editing skill
files.

## Advanced exercise -- List workflow

Create a second skill:

> Create a skill called Risk Intake. When I provide a project risk, help
> me normalize it into Title, Description, Impact, Probability,
> Mitigation, Owner, Target Date, and Status. Confirm the values with me
> before adding anything to the project Risks list.

This demonstrates a repeatable workflow rather than a reusable answer.

## Use cases

-   Contract/document review
-   Project status reporting
-   Content quality checks
-   Metadata/classification workflows
-   Standardized list intake
-   Document organization
-   Policy review
-   Repeatable team procedures

## Governance considerations

-   Skills inherit the user's permissions.
-   Skill files can be governed like other SharePoint content.
-   Treat skill instructions as managed business logic.
-   Assign an owner for important skills.
-   Review skills when the underlying process changes.
-   Test destructive or bulk workflows carefully.

## Skills vs. tools vs. knowledge

-   **Knowledge** gives the agent information to reference.
-   **Tools** connect an agent to actions/services.
-   **Skills** package reusable task-specific instructions and logic.
-   **Agent instructions** define broad behavior.

## Summary

Skills are valuable when a good prompt becomes a repeatable business
process. Instead of teaching every user the complete prompt, capture the
process once and make it reusable.

## References

-   Microsoft Learn -- Extend Copilot in SharePoint with skills:
    https://learn.microsoft.com/en-us/sharepoint/copilot-in-sharepoint-skills
-   Microsoft Learn -- Skills overview for agents:
    https://learn.microsoft.com/en-us/microsoft-copilot-studio/agents-experience/skills-overview
