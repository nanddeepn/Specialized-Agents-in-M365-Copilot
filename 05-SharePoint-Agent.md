# Lab 5 -- Create a SharePoint Agent

## Introduction

A SharePoint agent is a scoped AI assistant grounded in selected
SharePoint content. You can create one from a SharePoint site, document
library, list, or selected files, then customize its name, purpose,
sources, and behavior.

This is useful when a broad Copilot experience should become a focused
expert for a particular team, project, policy area, or knowledge
collection.

## Prerequisites

To create an agent in SharePoint, Microsoft currently documents:

-   A Microsoft Copilot license.
-   Edit permission on the SharePoint site.
-   Access to the files/pages/sites used as knowledge.
-   SharePoint agent capabilities available in your tenant.

Users only receive answers from content they already have permission to
access.

## Exercise scenario

Create an **HR Learning Agent** or **Project Knowledge Agent** using a
workshop SharePoint site.

Suggested content:

-   Employee onboarding guide
-   Leave policy
-   Learning catalog
-   FAQ
-   Project plan
-   Architecture overview
-   Meeting notes

Use fictional/non-sensitive workshop content.

## Exercise 1 -- Create the agent

From the SharePoint site:

1.  Open the site homepage.
2.  Select **New \> Agent**.
3.  Alternatively, open a document library/list and use the available
    **AI actions \> Create an agent** experience.
4.  Select the content/scope for the agent.
5.  Create the agent.

Depending on where you create it, SharePoint stores the agent as an
`.agent` file. Agents created from the site homepage are stored under
**Site Assets \> Copilots**.

## Exercise 2 -- Customize the agent

Use a clear configuration.

**Name:** Contoso Learning Guide

**Purpose:**

> Help employees find accurate answers about Contoso learning,
> onboarding, and internal development opportunities using approved
> SharePoint content.

**Behavior/instructions:**

> Answer using the configured SharePoint sources. Prefer current policy
> and learning documents. Cite or identify the source used when
> possible. If the answer is not supported by the configured content,
> say that you could not find it rather than inventing an answer. Keep
> answers concise and provide steps when the user asks how to complete a
> process.

**Starter prompts:**

-   What learning is available for new managers?
-   Summarize the onboarding process for a new employee.
-   Where can I find training about Microsoft 365 Copilot?
-   Compare the learning paths available for technical and non-technical
    employees.

## Exercise 3 -- Test grounding

Ask three questions:

1.  A question directly answered by a source.
2.  A question requiring information from two sources.
3.  A question not answered by any source.

The third test is especially important. Evaluate whether the agent
clearly communicates that the information is unavailable.

## Exercise 4 -- Permission test

If your workshop setup permits it:

1.  Add a document that only a subset of participants can access.
2.  Ask two users with different permissions the same question.
3.  Verify that the agent does not use content a user cannot access.

Never weaken production permissions merely to make an agent return more
information.

## Exercise 5 -- Share and surface the agent

Explore the options available in your tenant to:

-   Share the `.agent` file.
-   Use the agent from SharePoint.
-   Use/share it in Teams or Copilot Chat where supported.
-   Add an agent link to a SharePoint page.
-   Set an appropriate agent as the site's main agent if you are a site
    owner and the feature is available.

## Use cases

-   HR policy assistant
-   IT support knowledge assistant
-   Project knowledge agent
-   Sales enablement agent
-   Product documentation assistant
-   Learning assistant
-   Quality/process assistant
-   Department FAQ agent

## Design guidance

A good SharePoint agent has:

-   A narrow purpose
-   Curated knowledge
-   Clear instructions
-   Representative starter prompts
-   Permission-aware content
-   A named owner
-   A review process for outdated content

## Common mistake

Do not treat an agent as a fix for poor information architecture.
Duplicate, obsolete, contradictory, or badly permissioned SharePoint
content can reduce answer quality.

## Summary

SharePoint agents let business users turn existing SharePoint knowledge
into focused AI experiences without starting with custom code. The most
important design work is selecting trustworthy content and defining a
clear purpose.

## References

-   Microsoft Support -- Create an agent in SharePoint:
    https://support.microsoft.com/en-us/sharepoint/copilot-in-sharepoint/create-an-agent-in-sharepoint
-   Microsoft Support -- Manage agents in SharePoint:
    https://support.microsoft.com/en-us/sharepoint/copilot-in-sharepoint/manage-agents-in-sharepoint
