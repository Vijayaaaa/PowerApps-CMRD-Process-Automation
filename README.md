# Mobile Application & Workflow Automation for Inbound Logistics (CMRD)

## 📌 Executive Summary
This project showcases the design and deployment of a mobile application and automated workflow built using **Microsoft PowerApps** and **Power Automate**. The solution digitized the Central Material Receipt Discrepancy (CMRD) process across **31 pan-India sites**, replacing manual Excel logs with a streamlined mobile interface to track, flag, and resolve inbound discrepancies.

## 🏢 Business Problem
Previously, managing material receipt discrepancies during inbound logistics relied heavily on fragmented, manual paper trails and disconnected Excel trackers. This caused:
* Delayed communication between site operators and central teams.
* High turnaround times for closing discrepancy and shortage cases.
* Lack of centralized visibility into recurring vendor or transport discrepancies.

## ⚙️ Solution Architecture & Workflow

A custom low-code mobile application was engineered to capture discrepancy details directly at the dock, integrated with automated email notifications and routing via Power Automate.

```mermaid
flowchart TD
    A[Inbound Material Arrives at Dock] --> B{Discrepancy Identified?}
    B -- Yes --> C[Operator Logs Issue via Mobile PowerApp]
    B -- No --> D[Standard Inbound Processing Complete]
    C --> E[Automated Routing via Power Automate]
    E --> F[Instant Notification to Responsible Stakeholder]
    F --> G[Centralized Database Tracking & Resolution]
    G --> H[Power BI Discrepancy Analytics Dashboard]
