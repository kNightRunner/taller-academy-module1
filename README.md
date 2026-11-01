# Taller Academy — Module 1: Name the Value You Are Part Of

This public practice document focuses on two general GraphQL integration risks: **N+1 queries** and **conflicting mutations**. These are technical examples used to explain potential business impact, not claims about the architecture, customer data, or measured performance of any specific client.

## Exercise 1 — The two-sentence test

Our project helps digital applications retrieve and update information reliably, so people can use features without unnecessary delays or losing their changes. If repeated data requests slow the system down or simultaneous edits overwrite one another, users may experience slower responses or inconsistent information.

These two sentences intentionally avoid internal service names, unexplained acronyms, and implementation details.

## Exercise 2 — The stop test

**If the project froze for one month, who would notice first, and what exactly would they notice?**

The teams delivering features that depend on reliable data access and updates would probably notice first: performance problems and conflicting changes could remain unresolved, slowing development and testing. If these issues affected live usage, customer support and product teams might subsequently notice slow interactions, incorrect saved information, or more reports of failed updates. This is a risk-based assessment, not a report of observed incidents.

**Which business number does the work touch, even indirectly?**

Potentially relevant indicators include:

- **Response time for information retrieval** and the number of backend requests needed per user action (related to repeated queries).
- **Successful, conflict-safe update rate** and the volume of overwritten or rejected updates (related to concurrent mutations).
- **Support requests caused by slow or incorrect behavior**, if the client tracks them.

My team monitors query response times and error counts to assess service performance and stability. These indicators help identify problems that could affect the user experience. I am not including internal figures or baselines in this public document.

## Exercise 3 — One action

**What could my client manager accurately say about my contribution tomorrow, in two sentences?**

I work on assigned backend integration tasks and help verify that data retrieval and updates behave as expected. I have also reported failures in dependent services with documented request details, making those blockers visible to the teams responsible for investigating them.

**One action this week (date: November 3, 2026):**

Share a concise written update with my technical lead, manager, and relevant client stakeholders linking a recent integration task to the query response-time and error metrics that our team monitors. I will avoid confidential figures and use the update to make the impact of my work clearer.

## Two technical risks, explained in business terms

| Risk | What could go wrong for users? | What improvement would mean |
| --- | --- | --- |
| Repeated queries (N+1) | A list loads slowly because requesting more items creates more work for the system. | The same information can be retrieved with fewer unnecessary requests, potentially improving responsiveness and infrastructure efficiency. |
| Conflicting mutations | Two people change the same item and one person's changes replace the other's without warning. | Conflicts can be detected so people can review a newer change instead of silently losing work. |

These are possible benefits and should not be presented as measured outcomes without evidence.

## Self-check

- [x] I can state the project's value in two plain-language sentences.
- [x] I can explain who might notice a prolonged interruption and what they might notice.
- [x] I can identify business-relevant measurements related to the two risks.
- [x] I know that my team monitors query response times and error counts; specific internal values are intentionally omitted.
- [x] My technical lead, manager, and several client stakeholders are familiar with my work through daily meetings, Slack, and Jira updates.

**Visibility of my contribution:** My technical lead, manager, and multiple client stakeholders know the tasks I work on. I communicate progress and blockers in daily meetings, Slack messages, and Jira tickets.

**Privacy:** No client name, internal identifier, secret, proprietary code, or financial information is published.
