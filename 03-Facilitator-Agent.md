# Lab 3 -- Facilitator Agent in Microsoft Teams

## Introduction

Facilitator is an agent that participates in Microsoft Teams meetings.
It can generate real-time AI notes, track decisions and open questions,
help with the agenda and time, answer questions in meeting chat, capture
follow-up tasks, and support post-meeting work.

Unlike an agent you open for a private chat, Facilitator becomes part of
the collaborative meeting experience.

## Prerequisites

-   Microsoft Teams.
-   A scheduled Teams meeting.
-   A Microsoft Copilot license is required to add or turn on
    Facilitator.
-   Meeting policy/settings must allow Copilot and Facilitator.
-   Appropriate organizer/presenter permissions to turn Facilitator on
    during a meeting.
-   Transcription should be enabled when you want to interact with
    meeting context after the meeting.

Facilitator cannot be added to every meeting type; for example,
Microsoft documents restrictions for channel meetings, instant meetings,
and Teams calls.

## Exercise scenario

Run a 15-minute Contoso Retail project meeting with 3--5 workshop
participants.

Agenda:

1.  Review store-launch status -- 4 minutes
2.  Discuss top risks -- 5 minutes
3.  Agree actions -- 4 minutes
4.  Wrap-up -- 2 minutes

## Exercise 1 -- Add Facilitator while scheduling

1.  Open **Teams \> Calendar**.
2.  Create a new scheduled Teams meeting.
3.  Add participants and the agenda above.
4.  Open **Meeting options**.
5.  Under **Copilot and other AI**, ensure Copilot/Facilitator is
    allowed for the meeting.
6.  Turn **Facilitator** on.
7.  Save/send the meeting.

Alternatively, if permitted, an organizer or presenter can turn
Facilitator on during the meeting from **More actions**.

## Exercise 2 -- Run the meeting

During the meeting, deliberately include:

-   One decision
-   Two action items
-   One unresolved question
-   One risk
-   A discussion that begins to drift away from the agenda

Example conversation:

-   Decision: Pilot will start with five stores.
-   Action: Alex will prepare the training plan by Friday.
-   Action: Priya will validate device readiness.
-   Risk: Two stores have network-upgrade dependencies.
-   Open question: Should weekend support be included in the pilot?

Observe how Facilitator captures notes and meeting information.

## Exercise 3 -- Interact in chat

Where supported, @mention Facilitator in the meeting chat.

Try:

> @Facilitator summarize the decisions made so far.

Then:

> @Facilitator list the unresolved questions and the person who should
> follow up, if an owner was explicitly agreed.

And:

> @Facilitator create a concise executive-ready summary of the meeting.

Do not ask it to invent owners when the meeting did not assign them.

## Exercise 4 -- Tasks

Review the follow-up tasks captured in meeting notes. If task
synchronization is available in your tenant, review/accept the tasks and
observe the associated Planner experience.

Try asking Facilitator to create or update a meeting-related task if the
feature is available.

## Exercise 5 -- Post-meeting recap

After the meeting:

1.  Open the meeting chat.
2.  Open **Recap**.
3.  Review **Notes**.
4.  Compare AI-generated notes with what participants remember.
5.  Verify decisions, owners, deadlines, and unresolved questions.

If document generation is available, try:

> @Facilitator create a one-page project status document based on this
> meeting, including Decisions, Risks, Actions, Owners, and Due Dates.
> Do not invent missing information.

## Use cases

-   Project status meetings
-   Steering committee meetings
-   Planning workshops
-   Requirements discussions
-   Design reviews
-   Team stand-ups
-   Customer discovery meetings where organizational policy permits

## Best practices

-   Put a clear agenda in the meeting invite.
-   State decisions explicitly.
-   State action owners and due dates explicitly.
-   Tell participants that AI features are being used.
-   Verify notes before treating them as the official record.
-   Follow organizational recording, transcription, privacy, and
    compliance policies.

## Summary

Facilitator works best when the meeting itself is well structured. Clear
agendas, explicit decisions, and clear ownership improve the usefulness
of AI-generated notes and follow-up.

## References

-   Microsoft Support -- Facilitator in Microsoft Teams meetings:
    https://support.microsoft.com/en-us/teams/copilot/facilitator-in-microsoft-teams-meetings
-   Microsoft Support -- Meeting options in Teams:
    https://support.microsoft.com/en-us/teams/meetings/meeting-options-in-microsoft-teams
