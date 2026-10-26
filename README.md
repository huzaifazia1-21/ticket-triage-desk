# Ticket Triage Desk

> **Demonstration project.** Built with sample tickets from fictional customers to show how I approach support automation. Not client work.

A small support inbox that classifies each ticket, routes it to the right queue and drafts a first reply for an agent to edit and send.

## The problem it addresses

Support teams spend a lot of time reading tickets, deciding who should handle them and typing near-identical first replies. Urgent, business-blocking tickets can sit behind simple how-to questions.

## What it does

- Assigns a **category** (account access, email delivery, billing, bug/crash, how-to, performance)
- Sets a **priority** (P1 business-blocking, P2 degraded or broken feature, P3 question)
- Reads **sentiment**
- Routes to a **queue** (Tier 1 self-serve, Tier 2 auth, email, billing, engineering)
- Writes a one-line **summary for the agent** and a **suggested reply**
- Lets you paste a new customer message and see it triaged

## Try it

No install needed. Open `index.html` in any browser.

## How the triage works here

The four sample tickets come pre-triaged. New tickets you paste are classified by simple keyword rules in `ruleTriage()`, which keeps this demo free and self-contained. In a production build, that function would be replaced by a call to an AI model that returns the same fields (category, priority, sentiment, queue, summary, reply) as JSON, with a human reviewing replies before they are sent.

## Skills shown

Technical support workflows · ticket triage · support automation · reply drafting · JavaScript
