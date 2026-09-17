# Lab 4 -- Copilot Cowork

## Introduction

Copilot Cowork is designed to carry out multi-step work across Microsoft
365 rather than only tell you how to do it. Depending on enabled
capabilities and permissions, Cowork can work with email, calendars,
documents, spreadsheets, presentations, PDFs, meetings, apps, and other
Microsoft 365 context.

A key concept is **human control**: review the plan, inspect results,
and approve consequential actions before they happen.

## Prerequisites

Microsoft currently documents these core requirements:

-   Active Microsoft 365 Copilot license.
-   Modern browser such as Edge or Chrome.
-   Cowork available/enabled in the Microsoft Copilot environment.
-   Usage-based/Cowork billing configured.
-   Required permissions to the Microsoft 365 content and actions
    involved.

Features such as skills, plugins, model choice, and effort controls can
vary by rollout and tenant configuration.

## Exercise scenario

You are preparing for a Contoso Retail quarterly planning meeting. You
need to gather context, create a briefing, organize actions, and prepare
communications.

## Exercise 1 -- Start a Cowork session

1.  Open Microsoft Copilot and navigate to **Cowork**.
2.  Start with:

> Prepare me for the Contoso Retail quarterly planning meeting. First
> show me a plan of the work you intend to do. Do not send messages,
> create meetings, or modify files until I approve those actions.

3.  Review the proposed plan.
4.  Ask Cowork to change any unnecessary steps.

## Exercise 2 -- Add work context

Use **Add attachments / Add work context** to provide safe workshop
content, such as:

-   Previous meeting notes
-   Sales workbook
-   Project status document
-   Relevant emails or Teams conversations, if available in your demo
    environment

Prompt:

> Use the attached context to create a briefing with: current status,
> key metrics, decisions needed, risks, open actions, and five questions
> I should ask in the meeting. Clearly mark anything that is uncertain
> or missing.

## Exercise 3 -- Create an artifact

Prompt:

> Create a concise Word briefing document from the approved content. Use
> an executive summary followed by Metrics, Risks, Decisions Needed,
> Open Actions, and Questions.

Review the artifact before continuing.

## Exercise 4 -- Delegate follow-up work

Try a multi-step request:

> Based on the final briefing, draft a follow-up email for the project
> team, prepare an action tracker, and propose a 30-minute follow-up
> meeting next week. Show me each proposed action before anything is
> sent or scheduled.

Observe where Cowork asks for approval.

## Exercise 5 -- Build an app

If **Build an app** is available in your Cowork environment:

> Build a simple project action tracker for the quarterly planning team.
> Track action, owner, due date, status, priority, and notes. Include
> views for overdue and high-priority actions.

Review the generated solution and test it with sample data.

## What participants should learn

Cowork is different from ordinary chat because the goal is not just a
response. The goal can be a completed unit of work spanning several
steps and Microsoft 365 surfaces.

## Use cases

-   Meeting preparation
-   Inbox organization
-   Weekly planning
-   Event planning
-   Creating a package of documents
-   Coordinating follow-up work
-   Research-to-deliverable workflows
-   Building lightweight apps
-   Repetitive knowledge-work processes

## Safety and governance checklist

Before approving an action, ask:

-   Is the recipient correct?
-   Is the source content correct?
-   Is sensitive data being shared?
-   Is the generated document accurate?
-   Are meeting attendees and times correct?
-   Does the action comply with organizational policy?
-   Can the action be safely reversed?

## Best practices

-   Describe the desired outcome, not just a single click.
-   State constraints and approval boundaries.
-   Add only relevant work context.
-   Break very large assignments into milestones.
-   Review outputs before approving external actions.
-   Use explicit language such as "draft but do not send" when that is
    your intent.

## Summary

Cowork demonstrates the shift from conversational assistance to
delegated work. The user still owns the goal, context, permissions,
review, and approvals.

## References

-   Microsoft Learn -- Copilot Cowork overview:
    https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/
-   Microsoft Learn -- Get started with Copilot Cowork:
    https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/get-started
-   Microsoft Learn -- Use Copilot Cowork:
    https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/use-cowork
