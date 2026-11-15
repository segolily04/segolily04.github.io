---
layout: default
title: QBO AP Reconciliation Agent
---

# QBO AP Reconciliation Agent

An AI agent that monitors a receiving inbox for incoming invoice payment PDFs and reconciles them against a QuickBooks Online (QBO) account.

[View the code on GitHub](https://github.com/segolily04/QBO_AP_Reconcilation_Agent)

## The problem

Matching payment PDFs from email to open invoices in the books is slow, repetitive, and easy to get wrong.

## How it works

1. **Ingest:** the agent checks Gmail for new emails with invoice payment PDFs and downloads the attachments.
2. **Extract:** a Gemini AI model reads each PDF and pulls out the invoice details.
3. **Verify:** the agent checks the invoice balance in QuickBooks Online.
4. **Apply:** if everything lines up, it applies the payment. Guardrails stop the run if something looks off.

## Built with

Python, Gmail API, Google Gemini, QuickBooks Online API, and automated tests for the connectors and guardrails.

## Screenshots

![Screenshot placeholder: the agent running in the terminal](../assets/images/qbo-agent-terminal.png)

*Add a screenshot of a run (with any real client or vendor details blurred out).*

[Back to home](../index.html)
