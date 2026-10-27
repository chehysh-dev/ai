# Practical 4: Issue Management

> **Source:** AI Module 2 Lab Manual (Pages 13–14)  
> **Course:** BSc IT — Artificial Intelligence / Agile Project Management  
> **Platform:** Atlassian Jira Cloud  

---

## 1. Objective
To master issue management operations in Jira: creating an **Epic** and child issues, assigning issues to specific team members, configuring issue **Priority** and **Due Date**, and verifying that configured metadata displays accurately on board cards.

---

## 2. Requirements
1. Access to the **"AI learning"** (Key: **AL**) project board configured in Practicals 1–3.
2. At least one invited team member (from Practical 2) to demonstrate task assignment.
3. Appropriate permissions to create and edit issues.
4. An internet-connected web browser.

---

## 3. Procedure

### Part A: Create an Epic / Issue
*(Refer to PDF Page 13)*

#### Step 1: Open the Project Kanban Board
- **Navigation:** Top navigation bar -> **Spaces** (or **Projects**) -> **AI learning** -> Open **AL board**.
- **Action:** Locate the **BACKLOG** column on the board.
- **Expected result:** The Backlog column is displayed containing previously created issues (e.g., `AL-1: Customer Interaction`).

#### Step 2: Click the Create Button under Backlog
- **Navigation:** At the bottom of the **BACKLOG** column.
- **Action:** Click the **+ Create** button.
- **Expected result:** The inline card input box opens with an issue type dropdown.

#### Step 3: Select Issue Type (Epic)
- **Navigation:** Issue type selector icon next to the input field.
- **Action:** Click the icon and select **Epic** (or select **Task** / **Story** if Epics are created via the top menu).
- **Expected result:** The issue type icon changes to Epic (purple icon).

#### Step 4: Enter the Issue Summary
- **Navigation:** Inline text entry box.
- **Action:** Type the exact summary:
  ```text
  Specification understanding
  ```
- **Expected result:** The title is entered into the creation box.

#### Step 5: Commit Issue Creation
- **Navigation:** Inline text box.
- **Action:** Press the **Enter** key.
- **Expected result:** The issue is generated with unique key **`AL-2`** and title **"Specification understanding"** in the **BACKLOG** column.

---

### Part B: Configure Assignee, Due Date, and Priority
*(Refer to PDF Page 14)*

#### Step 6: Open the Issue Details Modal
- **Navigation:** Backlog column on **AL board**.
- **Action:** **Double-click** on the newly created card **`AL-2: Specification understanding`** (or single-click if using the side-drawer panel view).
- **Expected result:** The detailed issue modal/dialog window opens in the center of the screen displaying all fields (Status, Assignee, Labels, Due Date, Priority, Description, Child work items).

#### Step 7: Assign the Issue to a Team Member
- **Navigation:** Issue details window -> Right-hand **Details** panel -> Locate **Assignee**.
- **Action:** Click on the current assignee field (which defaults to *Unassigned* or *Automatic*). From the user dropdown list, select an active team member (e.g., your lab partner, `sayali birje`, or `chaitanya toraskar07`).
- **Expected result:** The selected user's profile avatar and name replace *Unassigned*.

#### Step 8: Configure the Due Date
- **Navigation:** Issue details window -> Right-hand Details panel -> Locate **Due date**.
- **Action:** Click the **Due date** field to open the calendar picker. Select a specific milestone date (e.g., `Sep 30, 2026` as illustrated in the manual).
- **Expected result:** The date `Sep 30, 2026` is saved in the Due date field.

#### Step 9: Configure Issue Priority
- **Navigation:** Issue details window -> Right-hand Details panel -> Locate **Priority**.
- **Action:** Click on the **Priority** dropdown (which defaults to *Medium*) and select **Highest** (represented by double red up-arrows `⬆️ Highest`).
- **Expected result:** The priority updates to **Highest**.

> **Jira Standard Priority Levels:**
> - 🔴 **Highest:** Critical blocker stopping production or development.
> - 🟠 **High:** Major feature or serious bug requiring quick resolution.
> - 🟡 **Medium (Default):** Normal development task with standard urgency.
> - 🔵 **Low:** Minor improvement or non-critical enhancement.
> - ⚪ **Lowest:** Cosmetic or trivial work items.

#### Step 10: Close the Issue Details Window
- **Navigation:** Top-right corner of the issue details modal dialog.
- **Action:** Click the close (**`X`**) button or click outside the dialog.
- **Expected result:** The dialog closes and you return to the **AL board**.

#### Step 11: Verify Updated Card on Dashboard
- **Navigation:** AL board -> **BACKLOG** column.
- **Action:** Inspect the **`AL-2: Specification understanding`** card.
- **Expected result:** All configured attributes are visibly rendered directly on the card face:
  - Issue Key: `AL-2`
  - Title: `Specification understanding`
  - Assignee Avatar: Visible in bottom-right corner
  - Priority Icon: Red double-arrow (`Highest`)
  - Due Date Badge: `Sep 30, 2026`

---

## 4. Verification
To verify that Practical 4 is completed properly:
1. Open **AL board**.
2. Locate card **`AL-2`**.
3. Confirm that the assignee avatar matches the user selected in Step 7.
4. Confirm that the priority icon shows **Highest**.
5. Confirm that the due date `Sep 30, 2026` appears on the card.
6. Click card **`AL-2`** to verify that all field values are preserved in the database.

---

## 5. Troubleshooting
| Issue | Cause | Solution |
| :--- | :--- | :--- |
| Due date field does not appear on the issue modal | Field is hidden in the project screen scheme | Click **Configure fields** at the top right of the issue dialog and check **Due date** to unhide it. |
| Cannot assign issue to a teammate | User has not verified their email invitation | Ensure the teammate accepted the invite or select yourself as assignee for testing. |
| Double-clicking card does not open popup | Browser pop-up blocker or click settings | Single click the issue card; a slide-out panel will open on the right side with identical fields. |
| Priority changes do not save | Connection dropped | Ensure a stable internet connection; Jira Cloud auto-saves field inputs as soon as clicked. |

---

## 6. Result
The issue **`AL-2: Specification understanding`** was successfully created, assigned to a verified project member, configured with a target **Due Date (Sep 30, 2026)** and **Highest Priority**, and verified on the Kanban board.

---

## 7. Viva Preparation

**Q1: What is the purpose of assigning an issue to a user in Jira?**  
*Answer:* Assigning an issue establishes accountability and ownership. The assignee is the individual team member responsible for working on the task, updating its status, and delivering the finished work.

**Q2: What is the significance of the "Due Date" field in Jira?**  
*Answer:* The Due Date indicates the deadline by which the task must be completed. It helps project managers track delivery timelines, generates calendar views, and triggers automated notifications when tasks are overdue.

**Q3: Name the five standard priority levels in Jira from highest to lowest.**  
*Answer:* 
1. Highest
2. High
3. Medium
4. Low
5. Lowest

**Q4: How do you associate a child Story or Task with an Epic in Jira?**  
*Answer:* Open the issue details modal and select the **Parent** (or **Epic Link**) field, then choose the desired Epic from the dropdown. Alternatively, create child issues directly from the Epic's "Child work items" section.

**Q5: Can an issue have multiple assignees in standard Jira?**  
*Answer:* By default, standard Jira enforces a single assignee per issue to ensure clear accountability, though multiple team members can be added as *Watchers* or contributors.

---

## 8. Practical Checklist
- [ ] Navigated to `AL board` Backlog.
- [ ] Created issue `Specification understanding` (`AL-2`).
- [ ] Opened issue details modal by double-clicking.
- [ ] Assigned the issue to a project team member.
- [ ] Set the Due Date to `Sep 30, 2026`.
- [ ] Set Priority to `Highest`.
- [ ] Closed modal and confirmed metadata is visible on the board card.
