# Lab 2 -- Researcher Agent

## Introduction

Researcher is a specialized Microsoft Copilot agent for complex,
multi-step research. It can combine information from the web and, in a
work context, Microsoft 365 information you have permission to access,
such as files, email, meetings, and chats. Its output is designed as a
structured, source-cited research report.

Use Researcher when the question needs investigation, synthesis,
comparison, and evidence rather than a quick answer.

## Prerequisites

-   Access to Microsoft Copilot.
-   An eligible Microsoft 365 Copilot subscription/license.
-   Researcher enabled in your environment.
-   Permission to the Microsoft 365 work sources you want to reference.
-   Web access enabled where your organization permits it.
-   Some advanced model-choice experiences can require additional admin
    configuration and/or Frontier availability.

## Exercise scenario

Contoso Retail is considering how AI could improve store operations.
Leadership wants an evidence-based report rather than a brainstorm.

## Exercise 1 -- Research a topic

1.  Open Microsoft Copilot.
2.  Under **Agents**, select **Researcher**.
3.  Enter:

> Research how generative AI and AI agents are being used in retail
> operations. Focus on store operations, customer service, inventory,
> workforce productivity, and risk. Use recent credible sources.
> Separate established capabilities from emerging or experimental uses.

4.  If Researcher asks clarifying questions, answer them.
5.  Review the generated report and citations.

### What to observe

-   Structure of the report
-   Source quality
-   Citations
-   Whether competing evidence is represented
-   Separation of facts, analysis, and recommendations

## Exercise 2 -- Combine work and web context

Attach or reference an internal strategy document that is safe for the
workshop, then prompt:

> Using our attached Contoso Retail strategy document and current
> external research, identify five AI opportunities that align with our
> stated priorities. For each opportunity, show the internal priority it
> supports, external evidence, expected value, risks, dependencies, and
> a practical pilot.

## Exercise 3 -- Ask Researcher to challenge itself

Prompt:

> Review the report for weak evidence, unsupported assumptions, outdated
> sources, and areas where reasonable experts may disagree. Add a
> section called "What could change this conclusion?"

This teaches participants to use AI as a research partner rather than an
unquestioned authority.

## Exercise 4 -- Research plan before report

Prompt:

> Before writing the report, propose a research plan for evaluating
> whether AI agents can reduce operational workload in retail. Include
> research questions, source types, evaluation criteria, and evidence
> gaps. Wait for my approval before proceeding.

Review the plan, refine it, and then ask Researcher to proceed.

## Optional -- Model choice, Critique, or Council

If these options are available in your tenant, demonstrate them after
the core lab. Availability can depend on Microsoft 365 Copilot
licensing, admin settings, supported clients, and Frontier/preview
status.

Use a complex question where multiple perspectives are valuable, then
compare:

-   A normal Researcher run
-   A Critique run
-   Other model-choice or multi-model options available in your tenant

Focus the discussion on source quality, completeness, disagreements, and
how the second-pass review changes the result.

## Strong prompt pattern

**Research question + Scope + Time period + Sources + Evaluation
criteria + Required sections + Evidence rules**

Example:

> Research the current enterprise adoption of AI agents in retail and
> logistics. Prioritize primary sources and reputable research published
> in the last 18 months. Compare benefits, implementation barriers,
> governance risks, and measurable outcomes. Cite every important
> factual claim and identify evidence gaps.

## Use cases

-   Market and industry research
-   Technology evaluation
-   Competitive landscape research
-   Policy and regulatory research
-   Vendor landscape analysis
-   Preparing an executive briefing
-   Synthesizing internal and external information
-   Building an evidence base before a strategic decision

## Researcher vs. Copilot Chat

Use Copilot Chat for quick questions, drafting, summarization, and
iterative conversation. Use Researcher when you need deeper
investigation, multiple sources, citations, and a report-like
deliverable.

## Best practices

-   Define the question before asking for the answer.
-   Specify recency when current information matters.
-   Ask for primary sources where possible.
-   Inspect citations.
-   Ask Researcher to surface uncertainty and conflicting evidence.
-   Do not assume a cited report is automatically correct.
-   Keep confidential organizational content within approved Microsoft
    365 boundaries.

## Summary

Researcher is designed for depth. Its value comes from combining
reasoning, source gathering, and structured synthesis. The best workshop
outcome is not simply a long report---it is learning how to frame a
research question and verify the evidence.

## References

-   Microsoft Support -- Get started with Researcher:
    https://support.microsoft.com/en-us/microsoft-365-copilot/get-started-with-researcher-in-microsoft-365-copilot
-   Microsoft Support -- Use model choice in Researcher:
    https://support.microsoft.com/en-us/office/use-model-choice-in-the-researcher-agent
