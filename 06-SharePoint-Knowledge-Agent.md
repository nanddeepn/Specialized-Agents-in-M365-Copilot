# Lab 6 -- Copilot in SharePoint (formerly Knowledge Agent)

## Introduction

Microsoft's current documentation refers to this experience as **Copilot
in SharePoint**. Earlier preview documentation and some administrative
PowerShell settings use the name **Knowledge Agent**. This lab keeps
"Knowledge Agent" in the title so participants can connect older demos
and terminology with the current product experience.

Copilot in SharePoint can help users work with SharePoint content and
create solutions using natural language, including sites, pages, lists,
libraries, reports, and Office content as capabilities roll out.

## Prerequisites

For the current preview experience, Microsoft documents:

-   An active Microsoft Copilot license.
-   Copilot in SharePoint available for the tenant/site.
-   Appropriate SharePoint permissions for the task.
-   Restricted Content Discovery must not suppress the AI experience on
    the site.
-   Supported tenant/environment and rollout.

Availability and usage limits can change during preview.

## Exercise scenario

Build a lightweight **Store Launch Workspace** using natural language.

The solution should contain:

-   Project information page
-   Store Launch Tracker list
-   Risks list
-   Document library
-   Useful views for managers

## Exercise 1 -- Open Copilot in SharePoint

1.  Open your workshop SharePoint site.
2.  Open the Copilot/AI experience from the SharePoint interface.
3.  Ask:

> Help me design a SharePoint solution for managing retail store
> launches. We need to track each store, launch date, region, launch
> manager, readiness status, risks, and key documents. First propose the
> solution structure. Do not create anything until I approve the plan.

4.  Review the proposed structure.
5.  Refine it before approving creation where the experience supports
    plan-and-build.

## Exercise 2 -- Create a list

Prompt:

> Create a Store Launch Tracker list with columns for Store Name,
> Region, Launch Date, Launch Manager, Readiness Status, Readiness
> Percentage, Risk Level, and Notes. Add realistic sample rows for ten
> fictional stores.

Review:

-   Column types
-   Choice values
-   Dates
-   Person fields
-   Sample data

## Exercise 3 -- Improve the list

Prompt:

> Create a manager-friendly view that shows launches in the next 60
> days, sorted by launch date, with the highest-risk launches easy to
> identify.

Then ask:

> Suggest two additional views that would help an operations manager and
> explain why.

## Exercise 4 -- Work with documents

In a workshop document library, ask Copilot in SharePoint to help with
supported content operations, for example:

> Summarize the documents in this library and identify the main project
> risks mentioned across them.

Or:

> Help me organize this library so project plans, store readiness
> documents, and training material are easier to find.

Only execute changes after reviewing what Copilot proposes.

## Exercise 5 -- Ask questions about the site

Try:

> What are the five most important things a new project manager should
> know from this site?

Then:

> Which information appears incomplete or contradictory across the
> available project content?

Validate the answer against the source material.

## Admin note

During preview, Microsoft documentation retains `KnowledgeAgent` naming
in SharePoint Online PowerShell parameters such as
`KnowledgeAgentScope`. This is an administrative compatibility detail
and helps explain why participants may see both terms.

## Use cases

-   Create a project workspace
-   Build lists and libraries
-   Improve information organization
-   Create views
-   Summarize site knowledge
-   Create pages and supporting content
-   Bootstrap a department solution
-   Accelerate prototyping before formal development

## Copilot in SharePoint vs. a SharePoint agent

**Copilot in SharePoint** is the broader AI experience for working with
and building on SharePoint.

A **SharePoint agent** is a configured, scoped assistant with selected
knowledge and behavior.

They complement each other: one helps you work/build; the other gives
users a reusable focused assistant.

## Summary

Copilot in SharePoint turns natural-language intent into SharePoint
work. Treat generated structures as a starting point: review
architecture, permissions, metadata, governance, accessibility, and
lifecycle requirements before production use.

## References

-   Microsoft Learn -- Get started with Copilot in SharePoint:
    https://learn.microsoft.com/en-us/sharepoint/copilot-in-sharepoint-get-started
-   Microsoft Support -- Getting started with Build in SharePoint:
    https://support.microsoft.com/en-us/sharepoint/get-started-with-sharepoint/getting-started-with-build-in-sharepoint
