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

Create an Excel or CSV file with below details:

```
Month,Region,Store,ProductCategory,Revenue,Cost,UnitsSold,CustomerSatisfaction
Jan-2026,North America,New York,Electronics,48500,35200,210,4.5
Jan-2026,Europe,London,Clothing,32600,21800,340,4.3
Jan-2026,Asia Pacific,Singapore,Home Appliances,41800,30100,185,4.6
Jan-2026,Middle East,Dubai,Electronics,52200,37400,225,4.7
Jan-2026,Africa,Johannesburg,Sports,27400,18900,290,4.2
Jan-2026,Latin America,Sao Paulo,Groceries,19800,14200,520,4.1
Jan-2026,North America,Toronto,Home Appliances,39500,28400,175,4.4
Jan-2026,Europe,Paris,Electronics,46700,33600,198,4.5
Jan-2026,Asia Pacific,Sydney,Sports,31200,21500,310,4.6
Jan-2026,Latin America,Mexico City,Clothing,28900,19400,325,4.2
Feb-2026,North America,Chicago,Groceries,22400,16100,580,4.3
Feb-2026,Europe,Berlin,Home Appliances,38600,27900,170,4.4
Feb-2026,Asia Pacific,Tokyo,Electronics,57400,40800,240,4.8
Feb-2026,Middle East,Abu Dhabi,Clothing,29800,20100,315,4.5
Feb-2026,Africa,Cape Town,Groceries,18300,13200,490,4.0
Feb-2026,Latin America,Buenos Aires,Sports,25100,17300,270,4.1
Feb-2026,North America,Vancouver,Sports,33400,22900,320,4.6
Feb-2026,Europe,Madrid,Clothing,30500,20700,330,4.3
Feb-2026,Asia Pacific,Seoul,Home Appliances,44900,32100,195,4.7
Feb-2026,Middle East,Riyadh,Electronics,49800,35900,215,4.4
Mar-2026,North America,Los Angeles,Electronics,53600,38100,230,4.6
Mar-2026,Europe,Amsterdam,Sports,34800,23700,335,4.5
Mar-2026,Asia Pacific,Mumbai,Clothing,27600,18500,360,4.2
Mar-2026,Middle East,Doha,Home Appliances,42100,30400,188,4.6
Mar-2026,Africa,Nairobi,Groceries,16900,12100,460,3.9
Mar-2026,Latin America,Santiago,Electronics,40200,29100,180,4.3
Mar-2026,North America,New York,Clothing,35400,23800,375,4.5
Mar-2026,Europe,London,Home Appliances,43500,31200,190,4.6
Mar-2026,Asia Pacific,Singapore,Electronics,55800,39600,235,4.8
Mar-2026,Africa,Lagos,Sports,23800,16600,255,4.0
Apr-2026,North America,Toronto,Sports,36100,24600,345,4.7
Apr-2026,Europe,Paris,Clothing,33700,22600,355,4.4
Apr-2026,Asia Pacific,Sydney,Home Appliances,46800,33400,205,4.7
Apr-2026,Middle East,Dubai,Groceries,25700,18400,610,4.5
Apr-2026,Africa,Johannesburg,Electronics,37900,27600,165,4.1
Apr-2026,Latin America,Sao Paulo,Clothing,29400,19800,340,4.2
Apr-2026,North America,Chicago,Home Appliances,41200,29700,182,4.4
Apr-2026,Europe,Berlin,Electronics,48900,34900,208,4.6
Apr-2026,Asia Pacific,Tokyo,Sports,38700,26100,350,4.8
Apr-2026,Latin America,Mexico City,Groceries,21300,15300,550,4.1
May-2026,North America,Vancouver,Electronics,51700,36900,220,4.7
May-2026,Europe,Madrid,Home Appliances,40100,28900,178,4.4
May-2026,Asia Pacific,Seoul,Clothing,36200,24100,385,4.6
May-2026,Middle East,Abu Dhabi,Sports,32900,22400,315,4.5
May-2026,Africa,Cape Town,Home Appliances,31500,23100,145,4.2
May-2026,Latin America,Buenos Aires,Electronics,39400,28600,175,4.3
May-2026,North America,Los Angeles,Groceries,24600,17500,625,4.5
May-2026,Europe,Amsterdam,Clothing,35100,23500,370,4.6
May-2026,Asia Pacific,Mumbai,Electronics,43800,31600,195,4.3
May-2026,Middle East,Riyadh,Home Appliances,45600,32700,200,4.5
Jun-2026,North America,New York,Sports,38200,25800,365,4.6
Jun-2026,Europe,London,Electronics,54800,38900,232,4.7
Jun-2026,Asia Pacific,Singapore,Groceries,28400,20100,680,4.8
Jun-2026,Middle East,Doha,Clothing,31800,21400,335,4.4
Jun-2026,Africa,Nairobi,Sports,22900,15900,245,4.1
Jun-2026,Latin America,Santiago,Home Appliances,35700,25800,160,4.3
Jun-2026,North America,Toronto,Electronics,50100,35800,215,4.6
Jun-2026,Europe,Paris,Groceries,26900,19100,640,4.5
Jun-2026,Asia Pacific,Sydney,Clothing,37400,24900,395,4.7
Jun-2026,Africa,Lagos,Electronics,34200,25100,150,4.0
Jul-2026,North America,Chicago,Clothing,36900,24700,390,4.5
Jul-2026,Europe,Berlin,Sports,37100,25100,355,4.6
Jul-2026,Asia Pacific,Tokyo,Home Appliances,49600,35200,218,4.9
Jul-2026,Middle East,Dubai,Electronics,58900,41600,250,4.8
Jul-2026,Africa,Johannesburg,Groceries,20100,14400,525,4.2
Jul-2026,Latin America,Sao Paulo,Sports,28600,19600,300,4.3
Jul-2026,North America,Vancouver,Home Appliances,42800,30700,190,4.7
Jul-2026,Europe,Madrid,Electronics,47200,33900,202,4.5
Jul-2026,Asia Pacific,Seoul,Groceries,26100,18500,620,4.6
Jul-2026,Latin America,Mexico City,Clothing,31200,20900,350,4.2
Aug-2026,North America,Los Angeles,Home Appliances,45200,32300,198,4.6
Aug-2026,Europe,Amsterdam,Electronics,51300,36500,220,4.7
Aug-2026,Asia Pacific,Mumbai,Sports,30400,20900,320,4.4
Aug-2026,Middle East,Abu Dhabi,Groceries,23900,17100,590,4.5
Aug-2026,Africa,Cape Town,Clothing,24500,16800,285,4.1
Aug-2026,Latin America,Buenos Aires,Home Appliances,33800,24600,152,4.2
Aug-2026,North America,New York,Electronics,57200,40500,245,4.8
Aug-2026,Europe,London,Sports,39600,26700,375,4.7
Aug-2026,Asia Pacific,Singapore,Clothing,38900,25800,410,4.8
Aug-2026,Middle East,Riyadh,Electronics,53100,37900,228,4.6
Sep-2026,North America,Toronto,Groceries,27100,19200,650,4.5
Sep-2026,Europe,Paris,Home Appliances,44700,31900,196,4.6
Sep-2026,Asia Pacific,Sydney,Electronics,56400,39900,238,4.8
Sep-2026,Middle East,Doha,Sports,34600,23400,330,4.5
Sep-2026,Africa,Nairobi,Clothing,21800,14900,260,4.0
Sep-2026,Latin America,Santiago,Groceries,19600,14100,505,4.2
Sep-2026,North America,Chicago,Sports,37300,25300,360,4.6
Sep-2026,Europe,Berlin,Clothing,35800,23900,380,4.5
Sep-2026,Asia Pacific,Tokyo,Groceries,29700,20900,710,4.9
Sep-2026,Africa,Lagos,Home Appliances,29800,21900,138,4.1
Oct-2026,North America,Vancouver,Clothing,38100,25400,405,4.7
Oct-2026,Europe,Madrid,Electronics,52600,37300,225,4.6
Oct-2026,Asia Pacific,Seoul,Sports,41200,27600,390,4.8
Oct-2026,Middle East,Dubai,Home Appliances,51400,36600,225,4.7
Oct-2026,Africa,Johannesburg,Electronics,40500,29400,178,4.3
Oct-2026,Latin America,Sao Paulo,Clothing,32600,21800,365,4.4
Oct-2026,North America,Los Angeles,Sports,41900,28200,400,4.7
Oct-2026,Europe,Amsterdam,Groceries,28300,19900,675,4.6
Oct-2026,Asia Pacific,Mumbai,Home Appliances,39700,28700,180,4.4
Oct-2026,Middle East,Abu Dhabi,Electronics,54900,39000,235,4.7
```

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
