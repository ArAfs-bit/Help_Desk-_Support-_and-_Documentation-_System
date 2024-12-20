# Help Desk Support System

## Overview
This project simulates a help desk support system using Jira and Confluence to manage support requests, troubleshooting documentation, and compliance guides. The project demonstrates key skills in configuring request types, workflows, automation, and dashboards to streamline IT support, aimed at improving compliance and support efficiency.

## Contents
- [Project Setup in Jira](#project-setup-in-jira)
  - [Project Dashboard](#project-dashboard)
  - [Custom Request Form: Request New Software](#custom-request-form-request-new-software)
  - [Workflow: Software Request](#workflow-software-request)
  - [Automation Rules](#automation-rules)
  - [Dashboard and Reporting](#dashboard-and-reporting)
- [Knowledge Base Integration with Confluence](#knowledge-base-integration-with-confluence)
- [Sample Issue and Resolution Workflow](#sample-issue-and-resolution-workflow)
- [Compliance Documentation](#compliance-documentation)
- [Conclusion](#conclusion)

## Project Setup in Jira

### Project Dashboard
This is the initial setup for the Help Desk Support System in Jira's Service Project. Here, we organize support channels, request types, and board queues to streamline customer support processes.

![Project Dashboard](Screenshots/project_dashboard.png)

### Custom Request Form: Request New Software
The **Request New Software** form allows users to submit requests for software licenses, providing essential details to ensure efficient processing.

- **Instructions**: Provides guidance on filling out the request.
- **Summary**: Brief description of the requested software and its intended purpose.
- **Description**: Detailed explanation of the need for the software, including usage and impact.

![Request Form Configuration](Screenshots/request_form_configuration.png)

- **Updated Form**:

![Request New Software Form](Screenshots/request_new_software_form1.png)

### Workflow: Software Request
The **Software Request Workflow** guides each request through stages from submission to completion. This helps track progress and ensures that all necessary approvals are obtained.

- **Open**: The initial status when a request is submitted.
- **In Progress**: The IT team is processing the request.
- **Awaiting Approval**: The request requires managerial or budget approval.
- **Approved**: Approval has been granted, and the request is ready for fulfillment.
- **Rejected**: The request was denied.
- **Completed**: The software has been provided, and the request is closed.

![Software Request Workflow](Screenshots/workflow_statuses.png)

### Automation Rules
Automation rules streamline the Software Request Workflow by handling common actions, such as assigning requests, moving requests to awaiting approval, and notifying users about status changes.

- **Auto-Assign New Requests**: Automatically assigns new software requests to a designated team member.
- **Move to Awaiting Approval**: Transitions requests to *Awaiting Approval* when specific criteria are met.
- **Auto-Close Completed or Rejected Requests**: Automatically closes requests after they’re marked as *Completed* or *Rejected* for 3 days.
- **Send Notification on Approval Status Change**: Notifies relevant users when the approval status is updated.

![Automation Rules](Screenshots/automation_rules.png)

### Dashboard and Reporting
A custom dashboard was set up to monitor key support metrics, showing issue statistics, recent activity, and ticket distribution.

![Dashboard Metrics](Screenshots/dashboard_metrics.png)

## Knowledge Base Integration with Confluence

1. In Confluence, create a knowledge base with FAQ and troubleshooting guides.
2. Link the Confluence space to the Jira project by using **Knowledge Base** under **Project Settings**.

   - **FAQ Example**: Answer common questions like Wi-Fi connection issues and password resets.

   ![FAQ Page in Confluence](Screenshots/confluence_faqs_page.png)

   - **Troubleshooting Guide**: Link the guide in Jira issues for direct access.

   ![Linked Knowledge Base in Jira](Screenshots/confluence_linked_to_jira.png)

## Sample Issue and Resolution Workflow

1. **Create an Issue** - Log an issue such as "Network Connectivity Issue" in Jira.
2. **Add Details** - Include impacted services, urgency, and a description of the problem.
3. **Attach Troubleshooting Guide** - Use Custom Fields for Troubleshooting Steps.

   ![Network Connectivity Issue](Screenshots/network_connectivity_issue.png)

## Compliance Documentation

The **Compliance Documentation** page in Confluence provides guidelines for policies like:
- **Security Policy**: Ensures secure handling of data and systems.
- **Data Privacy Guidelines**: Covers best practices for data privacy.
- **Software Usage Policy**: Outlines appropriate usage of software resources.

![Compliance Documentation in Confluence](Screenshots/compliance_documentation.png)

## Conclusion
This Help Desk Support System project illustrates the setup and management of an IT support desk using Jira and Confluence, focusing on structured request handling, automation, and documentation management. The system improves support efficiency, enhances compliance, and ensures the availability of critical information through an integrated knowledge base.

