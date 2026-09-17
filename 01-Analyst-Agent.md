# Lab 1 -- Analyst Agent

## Introduction

Analyst is a specialized Microsoft Copilot agent for data analysis.
Instead of manually inspecting rows, writing formulas, or building
charts first, you can attach business data and ask questions in natural
language. Analyst can calculate statistics, identify patterns and
outliers, compare segments, and present results using readable
explanations, tables, and visuals.

## When to use Analyst

Use Analyst when the primary problem is **understanding data** rather
than simply summarizing a document.

Good scenarios include:

-   Sales and revenue analysis
-   Cost and budget analysis
-   Customer or employee survey analysis
-   Trend and variance analysis
-   Operational KPI analysis
-   Identifying outliers
-   Comparing regions, products, teams, or time periods
-   Creating an executive summary from structured data

## Prerequisites

-   Work or school Microsoft 365 account.
-   Access to Microsoft Copilot.
-   Analyst must be available/enabled in your tenant.
-   A supported data file such as Excel or CSV.
-   Permission to access any cloud files you attach.

If Analyst is missing under **Agents**, your administrator might have
disabled it or your account might not meet the licensing requirements.

## Exercise scenario

You are the Operations Manager for Contoso Retail. You have monthly
sales data and want to understand regional performance.

Create an Excel or CSV file with these columns:

`Month, Region, Store, ProductCategory, Revenue, Cost, UnitsSold, CustomerSatisfaction`

Include at least 50--100 rows for a better exercise.

## Exercise 1 -- First analysis

1.  Open Microsoft Copilot.
2.  Under **Agents**, select **Analyst**.
3.  Select **+** and attach the sample Excel/CSV file.
4.  Enter:

> Analyze this dataset. Explain the data quality, key KPIs, important
> trends, and any unusual values. Do not make assumptions when data is
> missing.

5.  Review the response.
6.  Check whether Analyst identified the correct columns, date range,
    and metrics.

### What to observe

-   Did it calculate totals and averages correctly?
-   Did it identify missing or suspicious values?
-   Did it distinguish observations from explanations?
-   Were useful tables or charts produced?

## Exercise 2 -- Regional performance

Use this prompt:

> Compare revenue, gross margin, units sold, and customer satisfaction
> by region. Rank the regions by revenue, but also explain whether the
> highest-revenue region is healthy when margin and customer
> satisfaction are considered.

Then follow with:

> Create a concise executive summary with the five most important
> findings and the three questions leadership should investigate next.

## Exercise 3 -- Find anomalies

Prompt:

> Identify statistically unusual revenue, cost, margin, or unit-sales
> observations. Show the records involved, explain why each is unusual,
> and suggest business questions I should ask before treating it as a
> problem.

This is useful for teaching participants that an anomaly is a signal to
investigate, not automatically an error.

## Exercise 4 -- Trend analysis

Prompt:

> Analyze month-over-month trends by region and product category.
> Highlight sustained growth, sustained decline, sudden changes, and
> possible seasonality. Clearly separate facts visible in the data from
> hypotheses.

Follow with:

> Create a management-ready table with Metric, Finding, Evidence,
> Business Impact, and Recommended Follow-up.

## Exercise 5 -- Challenge Analyst

Ask:

> What additional data would materially improve this analysis? Explain
> why each missing field would help.

This helps participants learn that good analysis depends on good context
and data quality.

## Prompt pattern

A strong Analyst prompt usually contains:

**Goal + Data + Metrics + Dimensions + Comparison + Output format +
Guardrails**

Example:

> Using the attached sales workbook, compare Revenue and Margin across
> Region and Product Category for the last 12 months. Identify trends
> and anomalies, show supporting calculations, and provide an executive
> summary. Do not infer causes unless the data supports them.

## Use cases

  -----------------------------------------------------------------------
  Function                            Example
  ----------------------------------- -----------------------------------
  Finance                             Analyze budget vs. actuals

  Sales                               Compare pipeline or sales
                                      performance

  Operations                          Detect delays and operational
                                      anomalies

  HR                                  Analyze non-sensitive survey
                                      results

  Customer service                    Identify ticket-volume and
                                      resolution trends

  Project management                  Analyze milestones, risks, effort,
                                      and delivery data
  -----------------------------------------------------------------------

## Best practices

-   Give columns meaningful names.
-   Prefer clean tabular data.
-   State which KPIs matter.
-   Ask Analyst to show evidence for conclusions.
-   Validate calculations before making business decisions.
-   Ask follow-up questions rather than trying to put everything into
    one prompt.
-   Do not confuse correlation with causation.

## Summary

Analyst is most valuable when you have structured data and a business
question. It reduces the effort required to explore data, but the user
remains responsible for validating the data, calculations, assumptions,
and business interpretation.

## References

-   Microsoft Support -- Get started with Analyst in Microsoft Copilot:
    https://support.microsoft.com/en-us/microsoft-365-copilot/get-started-with-analyst-in-microsoft-365-copilot
-   Microsoft Support -- Agents built by Microsoft:
    https://support.microsoft.com/en-us/microsoft-365-copilot/agents-built-by-microsoft
