# Lab 8 -- SharePoint List to App

## Introduction

SharePoint and Microsoft Lists are often the fastest place to model
lightweight business data. When users need a richer user interface, you
can turn an existing list into an app experience with Power Apps.

This lab focuses on the practical path from **List → App**, then shows
how newer AI-assisted Power Apps experiences can accelerate app design
where available.

## Prerequisites

-   SharePoint Online or Microsoft Lists.
-   Permission to create/edit a list.
-   Access to Power Apps.
-   Permission to create an app in the relevant Power Platform
    environment.
-   Appropriate Power Apps licensing for the connectors/features used.
-   For newer AI/vibe experiences, availability and licensing depend on
    your tenant and preview status.

## Exercise scenario

Create a **Store Visit Tracker**.

### List schema

  Column             Type               Example
  ------------------ ------------------ ----------------------
  Title              Single line text   Pune Store Visit
  Store              Single line text   Pune Central
  VisitDate          Date               2026-09-18
  Visitor            Person             Workshop User
  VisitType          Choice             Audit
  Score              Number             88
  Status             Choice             Completed
  FollowUpRequired   Yes/No             Yes
  Notes              Multiple lines     Signage needs update

Suggested `VisitType` choices: Audit, Training, Launch, Support\
Suggested `Status` choices: Planned, In Progress, Completed, Cancelled

Add 10--20 sample rows.

## Exercise 1 -- Create the list

1.  Open the workshop SharePoint site.
2.  Select **New \> List**.
3.  Create a blank list named **Store Visit Tracker**.
4.  Add the columns above.
5.  Add sample items.

## Exercise 2 -- Create an app from the list

Depending on the current Microsoft Lists/SharePoint/Power Apps UI in
your tenant, use the available integration to create a Power App from
the existing list, or open Power Apps and create an app using the
SharePoint/Microsoft Lists data source.

Connect to the **Store Visit Tracker** list.

The generated app should provide the basic browse/view/edit experience.

## Exercise 3 -- Test the generated app

Verify that you can:

-   Browse visits.
-   Open a visit.
-   Create a visit.
-   Edit a visit.
-   Save changes back to the SharePoint list.

Check person, choice, date, number, and yes/no fields carefully.

## Exercise 4 -- Improve the app

Add/refine these requirements:

-   Home screen showing total visits.
-   Filter for `FollowUpRequired = Yes`.
-   Filter by visit status.
-   Highlight overdue planned visits.
-   Display average completed-visit score.
-   Add a button to create a new visit.

If using an AI-assisted Power Apps authoring experience, describe these
changes conversationally. Otherwise implement them using standard Power
Apps authoring.

## Exercise 5 -- Add business value

Extend the solution with one optional automation:

**When FollowUpRequired is Yes and a visit is completed, notify the
responsible person.**

Discuss whether this should be implemented in Power Apps or Power
Automate.

## Optional -- Power Apps vibe

If the Power Apps vibe preview is available, explore creating or
refining an app conversationally. Microsoft documentation for the 2026
preview also describes adding SharePoint data to the generated solution.

Compare:

-   Traditional List → Power App
-   AI-assisted Power Apps creation

Discuss speed, control, maintainability, ALM, licensing, and preview
limitations.

## Use cases

-   Inspections
-   Site visits
-   Issue tracking
-   Equipment requests
-   Training registrations
-   Onboarding checklists
-   Simple approval intake
-   Inventory processes
-   Project action tracking

## Architecture

``` text
User
  |
  v
Power App
  |
  v
SharePoint / Microsoft List
  |
  +----> Power Automate (optional)
  |
  +----> Notifications / Approvals / Other services
```

## Production considerations

Before using the pattern for a real business solution, review:

-   List size and delegation
-   Indexing
-   Permissions
-   Power Apps licensing
-   Environment strategy
-   DLP policies
-   Error handling
-   Accessibility
-   Mobile experience
-   ALM
-   Support ownership

## Summary

List-to-App is a strong low-code pattern when SharePoint is an
appropriate data source and users need a more guided experience than a
standard list form. AI-assisted authoring can accelerate the build, but
architecture and governance still matter.

## References

-   Microsoft Support -- Create a Power App for a list:
    https://support.microsoft.com/en-us/sharepoint/lists/documents-and-library/create-a-power-app-for-a-list
-   Microsoft Learn -- Power Apps vibe:
    https://learn.microsoft.com/en-us/power-apps/vibe/create-app-data-plan
