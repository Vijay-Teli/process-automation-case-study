# Process Automation Case Study (Power Automate + Pega RPA)

## Overview
Real-world case study documenting how I eliminated manual HR processes and improved onboarding compliance at a 2,000+ employee financial institution using Power Automate and Pega RPA.

## The Problem
New employee onboarding required manual account creation across multiple systems. HR staff had to:
- Manually create user accounts in the core banking system
- Enter the same employee data into 3+ separate platforms
- Track unique employee identifiers in spreadsheets to avoid duplicates
- Manually trigger DocuSign packets for new hire paperwork

This resulted in:
- 45+ minutes per new hire for account setup
- Frequent data entry errors and duplicate identifiers
- Delayed onboarding (1-3 days for full system access)
- Compliance risk from inconsistent access provisioning

## The Solution

### Automation 1: Pega RPA Bot for Account Creation
- Partnered with Business Analyst teams to design an RPA bot using Pega
- Bot automatically created new employee accounts in the core banking system when triggered by UKG Human Resources Information Systems new hire event
- Eliminated manual data entry for account creation
- Reduced user-creation errors to near zero
- Improved compliance by ensuring consistent provisioning

### Automation 2: Power Automate Workflows
- Built Power Automate flows to trigger DocuSign packets automatically when a new hire record was created in UKG
- Automated notification flows to IT, Security, and department managers when new accounts were provisioned
- Created approval workflows for access elevation requests

### Automation 3: Identifier Tracking Dashboard
- Built a Power BI dashboard to track and manage unique employee identifiers for the Talent Acquisition team
- Automated validation to ensure identifiers were not duplicated or reused
- Gave TA team real-time visibility into identifier availability

## Results
- Reduced new hire account setup from 45+ minutes to under 5 minutes
- Eliminated manual data entry errors in account creation
- Cut onboarding access delays from 1-3 days to same-day
- Improved audit compliance with consistent, automated provisioning
- Freed up HR staff time for higher-value work

## Before vs After

### Before (Manual Process)
1. HR receives new hire notification
2. HR manually enters data into core banking system (15 min)
3. HR manually enters data into email/AD system (10 min)
4. HR checks spreadsheet for available identifier (5 min)
5. HR manually sends DocuSign packet (5 min)
6. HR notifies IT and manager via email (5 min)
7. Wait for IT to provision additional access (1-3 days)
Total: 45+ minutes of manual work + 1-3 day wait

### After (Automated Process)
1. New hire record created in UKG HRIS
2. Pega RPA bot automatically creates banking system account
3. Power Automate triggers DocuSign packet
4. Power Automate notifies IT, Security, and manager
5. Identifier auto-assigned and tracked in Power BI dashboard
Total: Under 5 minutes, same-day access

## Tools Used
- Pega RPA (robotic process automation)
- Power Automate (workflow automation)
- Power BI (identifier tracking dashboard)
- UKG Pro HRIS (trigger system)
- DocuSign (document automation)
- SQL Server (data validation)

## Files in This Repo
- `process_flow_before.md` - Manual process documentation
- `process_flow_after.md` - Automated process documentation
- `metrics.md` - Detailed metrics and results

## Author
Vijay Teli | [LinkedIn](https://www.linkedin.com/in/vijay-teli-581854145/)
