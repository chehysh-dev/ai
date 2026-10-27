# Practical 3: Issue Types and Configuration

> **Source:** AI Module 2 Lab Manual (Pages 10–12)  
> **Course:** BSc IT — Artificial Intelligence / Agile Project Management  
> **Platform:** Atlassian Jira Cloud  

---

## 1. Objective
To understand Jira's issue hierarchy (Epic, Story, Task, Bug), create and configure an agile issue (**Task: "Customer Interaction"**) on the Kanban board, and configure project-level **Versions (Releases)** and **Components** in Project Settings.

---

## 2. Requirements
1. An active Jira Cloud account with the **"AI learning"** (Key: **AL**) project created in Practical 1.
2. Project Administrator or standard Member permissions.
3. Access to the Jira web interface via a web browser.
4. Basic understanding of agile artifacts (Stories, Epics, Releases, Components).

---

## 3. Jira Issue Types Hierarchy Explained

Before performing the procedure, understand the standard issue types available in Jira:

| Issue Type | Icon Representation | Definition & Agile Purpose |
| :--- | :---: | :--- |
| **Epic** | ⚡ / 🟣 Purple tag | A large body of work that can be broken down into smaller Stories or Tasks. Typically spans multiple sprints. |
| **Story** | 📗 Green bookmark | A user requirement expressed from an end-user perspective (*"As a [user], I want [feature] so that [benefit]"*). |
| **Task** | 🟦 Blue square | A standard piece of technical work that needs to be completed (e.g., database configuration, code refactoring). |
| **Bug** | 🔴 Red circle | A defect, error, or failure in the software that needs to be tracked and resolved. |
| **Sub-task** | 📋 Sub-item | A smaller piece of work within a parent Story or Task required to complete it. |

---

## 4. Procedure

### Part A: Create and Configure an Issue on the Board
*(Refer to PDF Pages 10–11)*

#### Step 1: Open the Project Kanban Board
- **Navigation:** Top navigation bar -> **Spaces** (or **Projects**) -> Select **AI learning** -> Open **AL board**.
- **Action:** Locate the **BACKLOG** column on the left side of the Kanban board.
- **Expected result:** The Backlog column displays an inline **+ Create** button at the bottom.

#### Step 2: Initiate Quick Issue Creation
- **Navigation:** AL board -> Under **BACKLOG** column.
- **Action:** Click the **+ Create** button (or click the top global navigation **+ Create** button).
- **Expected result:** An inline card input field with the placeholder *"What needs to be done?"* appears.

#### Step 3: Enter the Issue Summary
- **Navigation:** Inline card text box in Backlog.
- **Action:** Type the exact task summary:
  ```text
  Customer Interaction
  ```
- **Expected result:** The task title is typed into the issue creation box.

#### Step 4: Select the Issue Type
- **Navigation:** Dropdown menu next to the issue title field.
- **Action:** Click the issue type selector icon (which shows Story, Bug, or Task options). Select **Task** (`Task` blue icon).
- **Expected result:** The issue type is set to **Task**.

#### Step 5: Save and Commit the Issue
- **Navigation:** Issue creation box.
- **Action:** Press the **Enter** key (or click the blue checkmark/Create button).
- **Expected result:** The new issue card is created with key **`AL-1`** and title **"Customer Interaction"** in the **BACKLOG** column.

---

### Part B: Create and Configure Versions (Releases)
*(Refer to PDF Pages 11–12)*

Versions in Jira represent points-in-time software releases (e.g., `v1.0.0`, `Beta Release`).

#### Step 6: Navigate to Space / Project Settings
- **Navigation:** Left sidebar menu -> Click on **Space settings** (or **Project settings**).
- **Action:** In the settings sidebar, locate and click on **Versions** (or **Releases**).
- **Expected result:** The Releases management dashboard opens with the message *"This space has 0 releases"* and a **Create release** button.

#### Step 7: Click Create Release
- **Navigation:** Releases page header.
- **Action:** Click the blue **Create release** button.
- **Expected result:** The *"Create release"* modal form appears.

#### Step 8: Enter Release Details
- **Navigation:** *"Create release"* dialog.
- **Action:** Configure the following fields:
  1. **Name\*:** Enter `Release 1.0` (or `Version 1.0`).
  2. **Start date:** Select today's date using the calendar picker.
  3. **Release date:** Select a future milestone date (e.g., 2 weeks from today).
  4. **Description:** Enter `First production milestone containing core modules.`
  5. Click **Save**.
- **Expected result:** The release is created and listed in the Releases table under the **Unreleased** tab with its start date, target release date, and progress bar (0% completed).

---

### Part C: Create and Configure Components
*(Refer to PDF Page 12)*

Components are subsections of a project used to group issues into logical functional areas (e.g., *Frontend*, *Backend*, *Database*, *API*).

#### Step 9: Open Components Settings
- **Navigation:** Left sidebar menu -> **Space settings** -> Click on **Components**.
- **Action:** Wait for the Components management table to load.
- **Expected result:** The Components page opens showing existing components or an empty state with a **Create component** button.

#### Step 10: Click Create Component
- **Navigation:** Components page header.
- **Action:** Click the blue **Create component** button.
- **Expected result:** The *"Create component"* modal form opens.

#### Step 11: Configure Component Details
- **Navigation:** *"Create component"* modal.
- **Action:**
  1. **Name\*:** Enter `User Interface` (or `Frontend Module`).
  2. **Description:** Enter `Handles client-facing UI pages, forms, and interaction.`
  3. **Component Lead:** Select your account name from the dropdown.
  4. **Default Assignee:** Select **Component Lead** (or **Project Default**).
  5. Click **Save**.
- **Expected result:** The component is saved and displayed in the Components table with its name, description, lead, and default assignee.

---

## 5. Verification
To confirm successful completion of Practical 3:
1. **Board Check:** Open **AL board**. Verify that issue **`AL-1: Customer Interaction`** is visible in the **BACKLOG** column.
2. **Releases Check:** Go to **Space settings -> Releases (Versions)**. Verify that `Release 1.0` is listed with its scheduled dates.
3. **Components Check:** Go to **Space settings -> Components**. Verify that `User Interface` is listed with you as the Component Lead.

---

## 6. Troubleshooting
| Issue | Cause | Solution |
| :--- | :--- | :--- |
| Issue type *"Epic"* is not visible in the dropdown | Kanban boards may hide Epics from inline quick-create | Click the top global **+ Create** button in the main navigation bar to select **Epic** from the full modal. |
| Cannot find *"Versions"* in settings | The menu item may be named *"Releases"* | In modern Jira Cloud, Versions are labeled as **Releases** in the sidebar. |
| *"Component name must be unique"* error | A component with that name already exists | Use a descriptive unique name like `Frontend-V1` or `UI-Component`. |
| Cannot set Component Lead | Lead user lacks project browse permissions | Assign a team member who has verified access to the project. |

---

## 7. Result
An issue of type **Task** titled **"Customer Interaction"** (`AL-1`) was successfully created on the Kanban board. Project milestones were configured via **Releases (Versions)**, and functional grouping was established by creating a project **Component**.

---

## 8. Viva Preparation

**Q1: What is the difference between an Epic, a Story, and a Task in Jira?**  
*Answer:* An **Epic** is a large goal or feature that spans multiple sprints and contains multiple stories. A **Story** is an end-user requirement focused on delivering business value. A **Task** represents specific technical work needed to support a story or maintenance activity.

**Q2: What is a Jira Component and why is it used?**  
*Answer:* A Component is a project subsection used to organize issues into functional sub-modules (such as UI, Backend, Security, Database). It helps filter issues, generate component-specific reports, and automatically route issues to specific Component Leads.

**Q3: What is a Jira Version / Release?**  
*Answer:* A Version (or Release) represents a scheduled software release or milestone. Issues assigned to a version are tracked together to measure completion progress against target delivery dates.

**Q4: Can an issue belong to multiple components in Jira?**  
*Answer:* Yes. Jira allows an issue to be tagged with multiple components if the task affects more than one technical subsystem.

**Q5: What happens when an issue is assigned to a Component with a configured "Default Assignee"?**  
*Answer:* When the issue is created and that component is selected, Jira can automatically assign the issue to the designated Component Lead, streamlining triage.

---

## 9. Practical Checklist
- [ ] Navigated to the `AL board` Backlog.
- [ ] Created a new Task named `Customer Interaction` (`AL-1`).
- [ ] Verified the task appears in the Backlog column.
- [ ] Opened Space settings -> Releases (Versions).
- [ ] Created `Release 1.0` with start and release dates.
- [ ] Opened Space settings -> Components.
- [ ] Created a new component named `User Interface`.
