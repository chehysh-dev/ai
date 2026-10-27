# SOURCE AND ASSUMPTIONS: AI MODULE 2 (JIRA PRACTICALS)

This document provides a technical audit trail mapping the step-by-step instructions in this repository directly to the source document (**AI module 2.pdf**, 28 pages), documenting clarifications made for modern Jira Cloud interfaces, and highlighting limitations where details could not be determined from the raw screenshots.

---

## 1. Primary Source Mapping

| Practical | PDF Page Range | Documented Activities in Source PDF | Source Entities & Key Values |
| :--- | :---: | :--- | :--- |
| **Practical 1** | Pages 1–7 | - Google search -> Atlassian Jira site.<br>- Google OAuth signup with Gmail ID.<br>- Work category: *"Project management"*.<br>- Onboarding template: *"Kanban"*, space name: *"My First Project"*.<br>- Create Space -> Kanban -> Company-managed -> Name: *"AI learning"*, Key: `AL`.<br>- Space settings -> Details configuration. | - Account: `sayali birje`<br>- Site URL: `birjesayali20-1788950198690.atlassian.net`<br>- Project Name: `AI learning`<br>- Key: `AL`<br>- Type: `Company-managed` |
| **Practical 2** | Pages 8–9 | - Open `AL board` -> Click *"Add people"*.<br>- Enter email -> select role -> click *"Add 1 Person"*.<br>- Dialog confirms 1 person added and 1 licence consumed.<br>- Manage access via space settings. | - Dialog: *"Add people to AI learning"*<br>- Teammate: `sayali.birje@avc.ac.in`<br>- Role: `Member` / `Administrator` |
| **Practical 3** | Pages 10–12 | - Backlog -> Click `+ Create` -> Summary: *"Customer Interaction"* -> Type: `Task` -> Key: `AL-1`.<br>- Space settings -> Versions (Releases) -> Click *"Create release"*.<br>- Space settings -> Components -> Click *"Create component"*. | - Issue: `AL-1: Customer Interaction`<br>- Type: `Task`<br>- Settings: Versions & Components |
| **Practical 4** | Pages 13–14 | - Backlog -> `+ Create` -> Type: `Epic` -> Summary: *"Specification understanding"* -> Key: `AL-2`.<br>- Double-click card -> modal popup.<br>- Assignee: `chaitanya toraskar07` / `sayali birje`.<br>- Due date: `Sep 30, 2026`.<br>- Priority: `Highest`.<br>- Card face verifies all fields on board. | - Issue: `AL-2: Specification understanding`<br>- Priority: `Highest`<br>- Due date: `Sep 30, 2026`<br>- Assignee: team member |
| **Practical 5** | Pages 15–17 | - Space settings -> Workflows.<br>- Add workflow -> Add existing -> *"classic default workflow"*.<br>- Assign to Bug, Story, Task, Sub-task.<br>- View Diagram: Open, In Progress, Resolved, Reopened, Closed.<br>- Add Transition: `Open` -> `In Progress`.<br>- Add Rule / Condition: Restrict transition.<br>- Update workflow -> Publish draft -> Associate -> Acknowledge. | - Scheme: `AL: Software Simplified Workflow Scheme`<br>- Workflow: `classic default workflow`<br>- Transition: `Open` -> `In Progress`<br>- Rule: Restrict transition |
| **Practical 6** | Pages 18–23 | - Create Space -> Scrum -> Company-managed.<br>- Project Name: *"Online Shopping Site"*, Key: `OSS`.<br>- Go to Backlog -> `OSS Sprint 1`.<br>- Create 5 Stories with points:<br>  1. User Registration (3)<br>  2. User Login (3)<br>  3. Product Catalog (5)<br>  4. Shopping Cart (8)<br>  5. Checkout Process (13)<br>- Total Story Points: 32.<br>- Start Sprint: 2 weeks duration -> Complete Sprint -> Summary & Reports. | - Project: `Online Shopping Site`<br>- Key: `OSS`<br>- Sprint: `OSS Sprint 1`<br>- Total Points: 32 (3, 3, 5, 8, 13)<br>- Duration: 2 weeks |
| **Practical 7** | Pages 24–28 | - Create Space -> Kanban -> Company-managed.<br>- Project Name: *"AI Education Bot"*, Key: `ED` / `AEB`.<br>- Backlog -> `+ Create` -> *"Create user registration and login system"* (`ED-1`).<br>- Assignee: `Sayali Birje`, Priority: `High`, Due date set.<br>- Move across columns: Selected for Development -> In Progress -> Done.<br>- Reports -> More reports -> Agile -> Cumulative Flow Diagram & Control Chart. | - Project: `AI Education Bot`<br>- Key: `ED` (or `AEB`)<br>- Issue: `ED-1: Create user registration and login system`<br>- Reports: CFD & Control Chart |

---

## 2. Necessary Interface & Terminology Clarifications

### A. "Spaces" vs. "Projects"
- **Observation in PDF:** In several screenshots (Pages 2–7, 11–12, 18, 24), the top navigation bar and settings menu use the label **"Spaces"** (e.g., *"Name your space"*, *"Space settings"*), while in other views (Pages 15–16), the breadcrumb displays **"Project settings"**.
- **Clarification:** Atlassian periodically experiments with labeling in Jira Cloud. In Jira Work Management and Jira Service Management, workspaces are occasionally labeled as *"Spaces"*, whereas in standard Jira Software, they are labeled as **"Projects"**. Both terms refer to the exact same administrative container. Throughout these practical guides, instructions explicitly indicate: **"Spaces (or Projects)"** and **"Space settings (or Project settings)"**.

### B. "Releases" vs. "Versions"
- **Observation in PDF:** Page 11 refers to the section as *"1. VERSIONS"*, but the button in the screenshot on Page 12 is explicitly labeled **"Create release"**, with an administrative notice: *"Spaces will be limited to 15,000 releases"*.
- **Clarification:** In Jira, "Releases" and "Versions" are synonymous terms for shipping software milestones. The documentation retains both terms so students can locate the feature regardless of whether their interface displays *"Versions"* or *"Releases"*.

### C. "Rules" vs. "Conditions"
- **Observation in PDF:** Page 17 instructs: *"Click 'add rule' -> select any rule type"*. In classic Jira Server / Data Center, these were labeled as **Conditions**, **Validators**, and **Post Functions**, whereas in Jira Cloud, Atlassian unified these under **"Rules"**.
- **Clarification:** The practical guide explains both terms so that students working on Jira Cloud or older server editions understand that a *"Rule"* in Cloud enforces transition conditions.

---

## 3. Details That Could Not Be Determined from Source Screenshots

1. **Exact Email Domain in Page 8:** In Practical 2, the email address `sayali.birje@avc.ac.in` is partially visible in the invite modal and top browser tabs. Rather than requiring students to use this exact college domain, the guide explains that students must provide a valid email address they control to avoid licence wastage.
2. **Component Fields on Page 12:** The screenshot on Page 12 shows the button *"Click Create Component -> Enter details. Click Save."* but does not display the open modal. Standard Jira component fields (**Name**, **Description**, **Component Lead**, and **Default Assignee**) have been provided based on standard Atlassian specifications and clearly labeled as standard fields.
3. **Control Chart Exact Data on Page 28:** Page 28 shows the navigation button to the Control Chart and Cumulative Flow Diagram, but the final rendered data curve reflects mock data generated by Atlassian. The guide explains how the chart evaluates Cycle Time, Rolling Average, and Standard Deviation without fabricating specific numerical test data.
