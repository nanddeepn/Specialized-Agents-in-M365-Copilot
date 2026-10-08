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

Create an **Talent Finder Agent** using a workshop SharePoint site.

- Create a SharePoint site.
- Create a document library or use the out of box "Shared Documents" library.
- Upload sample resumes from [here](/assets/Resumes/)

## Exercise 1 -- Create the agent

From the SharePoint site:

1.  Open the site homepage.
2.  Select **New \> Agent**.
3.  Alternatively, open a document library/list and use the available **AI actions \> Create an agent** experience.
4.  Select the content/scope for the agent.
5.  Create the agent.

Depending on where you create it, SharePoint stores the agent as an
`.agent` file. Agents created from the site homepage are stored under
**Site Assets \> Copilots**.

## Exercise 2 -- Customize the agent

Use a clear configuration.

**Name:** Talent Finder Agent

**Purpose:**

> Helps HR and recruitment teams discover suitable candidates from resumes stored in SharePoint. It can search and analyze resumes across different languages and identify candidates based on skills, experience, technologies, roles, education, certifications, and other job-related criteria.

**Welcome message:**

> Welcome to Talent Finder! 
> 👋 I can help you discover candidates from the resumes available in SharePoint. Tell me the skills, experience, role, technology, location, or other job-related criteria you're looking for, and I'll help identify relevant candidates.

**Starter prompts:**

> Suggest candidates with SQL experience.

> Find candidates with 5+ years of experience in .NET and Azure.

> Suggest candidates suitable for a Senior Data Engineer role.

**Agent instructions:**

> You are an HR Talent Finder Agent that helps recruiters find suitable candidates from resumes stored in SharePoint.
> - Search and understand resumes across different languages.
> - Match candidates based on skills, experience, roles, technologies, certifications, education, and other job-related criteria.
> - Consider related terminology and skill variations while clearly distinguishing exact and related matches.
> - Rank candidates based only on evidence available in their resumes.
> - Present matches with Candidate Name, Relevant Skills, Experience, Role, and Why They Match.
> - Never invent missing candidate information.
> - Do not use sensitive or protected personal characteristics when evaluating candidates.
> - Keep recommendations objective, evidence-based, and easy for recruiters to verify.


## Exercise 3 -- Test grounding

Ask a question:

> We are looking for a Senior Data Engineer with 5+ years of experience, strong SQL skills, Azure experience, and knowledge of Python. Find the best matching candidates and explain why each candidate matches.


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

- [Create an agent in SharePoint](https://support.microsoft.com/en-us/sharepoint/copilot-in-sharepoint/create-an-agent-in-sharepoint?WT.mc_id=M365-MVP-5003693)
- [Manage agents in SharePoint](https://support.microsoft.com/en-us/sharepoint/copilot-in-sharepoint/manage-agents-in-sharepoint?WT.mc_id=M365-MVP-5003693)
