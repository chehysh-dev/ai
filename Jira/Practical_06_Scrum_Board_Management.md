# Practical 6: Scrum Board Management

> **Source:** AI Module 2 Lab Manual (Pages 18–23)  
> **Course:** BSc IT — Artificial Intelligence / Agile Project Management  
> **Platform:** Atlassian Jira Cloud  

---

## 1. Objective
To create and configure a dedicated agile **Scrum project and board** (**"Online Shopping Site"**, Key: **`OSS`**), populate the backlog with estimated user stories using standard Fibonacci **Story Points** (3, 3, 5, 8, 13), plan and initiate an active **Sprint (OSS Sprint 1)**, complete the sprint, and analyze generated **Sprint Reports** and **Burndown Charts**.

---

## 2. Requirements
1. An active Jira Cloud administrator account.
2. An internet-connected computer with a modern web browser.
3. Theoretical understanding of the Scrum framework:
   - **Product Backlog:** Prioritized list of all requirements and features.
   - **Sprint:** A time-boxed iteration (typically 1–4 weeks) during which specific work is delivered.
   - **Story Points:** An estimation unit representing the relative effort, complexity, and uncertainty of a story.
   - **Sprint Report / Burndown Chart:** Visual metrics showing work completed vs. remaining work over time.

---

## 3. Procedure

### Part A: Create and Configure a Scrum Project & Board
*(Refer to PDF Pages 18–20)*

#### Step 1: Open the Project Creation Menu
- **Navigation:** Top navigation bar -> Click **Spaces** (or **Projects**) -> Click **+ Create space** (or **Create project**).
- **Action:** Open the template catalog.
- **Expected result:** The project template categories (Software development, Work management, Service management) appear.

#### Step 2: Select the Scrum Template
- **Navigation:** Template library -> Categories -> Select **Software development** (or **Work management**).
- **Action:** Locate and click on the **Scrum** template (*"Plan, track, and execute work using sprints and a backlog"*).
- **Expected result:** The Scrum template details and issue type breakdown (Epic, Story, Task, Bug, Sub-task) are shown.

#### Step 3: Confirm Template Selection
- **Navigation:** Template details page.
- **Action:** Click the blue **Use template** button at the bottom right.
- **Expected result:** The project configuration form opens.

#### Step 4: Configure Project Details
- **Navigation:** *"Name your space / project"* form.
- **Action:**
  1. In the **Name\*** field, enter:
     ```text
     Online Shopping Site
     ```
  2. The **Key\*** field auto-populates as `OSS` (or enter `OSS` manually).
  3. Under **How your space is managed\***, select: **Company-managed**.
  4. Click **Next**.
- **Expected result:** Jira provisions the Scrum architecture.

#### Step 5: Skip Team Invitations
- **Navigation:** *"Bring your team along"* screen.
- **Action:** Click **I'll do this later**, then click **Done**.
- **Expected result:** A notification displays *"Jira space successfully created"*, and you are redirected to the **OSS board**.

#### Step 6: Inspect the Initial Scrum Board
- **Navigation:** Project dashboard -> **OSS board**.
- **Action:** Observe the board tabs on the left sidebar:
  - **Summary**
  - **Timeline**
  - **Backlog**
  - **Active sprints**
  - **Reports**
- **Expected result:** The Active Sprints board displays three default columns: `TO DO`, `IN PROGRESS`, and `DONE` with a prompt: *"Get started in the backlog. Plan and start a sprint to see work here."*

---

### Part B: Populate Backlog, Estimate Story Points, and Start Sprint
*(Refer to PDF Pages 20–23)*

#### Step 7: Open the Scrum Backlog
- **Navigation:** Left sidebar menu -> Click on **Backlog** (or click the blue **Go to Backlog** button on the board).
- **Action:** Wait for the backlog view to load.
- **Expected result:** The backlog interface loads, displaying the **OSS Sprint 1** planning container at the top and the open **Backlog** section below it.

#### Step 8: Create the 5 Required User Stories
- **Navigation:** Backlog view -> Inside the **OSS Sprint 1** container -> Click **+ Create**.
- **Action:** Create the following 5 user stories sequentially. Ensure the issue type is set to **Story** (`📗 Story`):
  1. Type `User Registration` and press **Enter** (Created as `OSS-1`).
  2. Type `User Login` and press **Enter** (Created as `OSS-2`).
  3. Type `Product Catalog` and press **Enter** (Created as `OSS-3`).
  4. Type `Shopping Cart` and press **Enter** (Created as `OSS-4`).
  5. Type `Checkout Process` and press **Enter** (Created as `OSS-5`).
- **Expected result:** All five stories are listed inside the **OSS Sprint 1** container.

#### Step 9: Assign Story Points to Each Story
*(Using the exact Fibonacci point values from PDF Page 21)*

- **Navigation:** Click on each story card in the sprint container to open its quick details or edit the story points badge on the right of the row.
- **Action:** Assign the respective Story Points:
  - `OSS-1: User Registration` -> Set Story Points to **3**
  - `OSS-2: User Login` -> Set Story Points to **3**
  - `OSS-3: Product Catalog` -> Set Story Points to **5**
  - `OSS-4: Shopping Cart` -> Set Story Points to **8**
  - `OSS-5: Checkout Process` -> Set Story Points to **13**
- **Expected result:** The sprint header updates to show:
  ```text
  OSS Sprint 1 (5 work items) | Estimate: 32 Story Points
  ```
  *(Calculation: 3 + 3 + 5 + 8 + 13 = 32 points total).*

#### Step 10: Click Start Sprint
- **Navigation:** Top-right corner of the **OSS Sprint 1** header container.
- **Action:** Click the blue **Start sprint** button.
- **Expected result:** The *"Start Sprint"* configuration modal opens.

#### Step 11: Configure Sprint Parameters
- **Navigation:** *"Start Sprint"* dialog.
- **Action:**
  1. **Sprint name\*:** Verify `OSS Sprint 1`.
  2. **Duration\*:** Select **2 weeks** from the dropdown.
  3. **Start date:** Confirm current date/time.
  4. **End date\*:** Automatically calculates to 14 days from start.
  5. **Sprint goal:** Enter `Complete core shopping and checkout workflow.`
  6. Click the blue **Start** button.
- **Expected result:** The sprint activates, and Jira automatically redirects you to the **Active sprints** board.

#### Step 12: Inspect the Active Sprints Board
- **Navigation:** Left sidebar -> **Active sprints** (or `OSS board`).
- **Action:** Observe the board columns.
- **Expected result:** All 5 stories (`OSS-1` through `OSS-5`) are actively rendered in the **TO DO** column with their story point badges visibly attached.

---

### Part C: Simulate Work Progress, Complete Sprint & Generate Reports
*(Refer to PDF Pages 22–23)*

#### Step 13: Transition Stories Across Board Columns
- **Navigation:** Active sprints board.
- **Action:** Drag and drop the cards to simulate agile team progress:
  - Drag `OSS-1 (User Registration)` and `OSS-2 (User Login)` from `TO DO` -> `IN PROGRESS` -> `DONE`.
  - Drag `OSS-3 (Product Catalog)` from `TO DO` -> `IN PROGRESS` -> `DONE`.
  - Drag `OSS-4 (Shopping Cart)` and `OSS-5 (Checkout Process)` to `IN PROGRESS` (or move all to `DONE`).
- **Expected result:** Stories transition into their respective columns, updating real-time team burn-down data.

#### Step 14: Complete the Sprint
- **Navigation:** Top-right corner of the Active Sprints board.
- **Action:** Click the **Complete sprint** button.
- **Expected result:** The *"Complete OSS Sprint 1"* summary dialog opens showing the number of completed issues and any uncompleted issues (with an option to move uncompleted work back to the Backlog or a future sprint).

#### Step 15: Confirm Sprint Completion
- **Navigation:** Complete sprint dialog.
- **Action:** Click the blue **Complete** button.
- **Expected result:** The sprint is closed, and Jira automatically generates agile metrics.

#### Step 16: Review Project Summary Metrics
- **Navigation:** Left sidebar -> Click **Summary**.
- **Action:** Inspect the high-level project analytics cards.
- **Expected result:** The Summary page displays:
  - `Completed in the last 7 days` count.
  - `Updated in the last 7 days` count.
  - `Created in the last 7 days` count.
  - `Status overview` donut chart showing the proportion of items in Done, In Progress, and To Do.

#### Step 17: Generate and Inspect the Sprint Report
- **Navigation:** Left sidebar -> Click **Reports**.
- **Action:** Under the **Agile** section, click on **Sprint Report** (or **Burndown Chart**).
- **Expected result:** The Sprint Report loads, displaying:
  - The **Burndown Chart** graphing committed story points vs. actual burn-down curve against the guideline.
  - A table listing **Completed Issues** (`OSS-1`, `OSS-2`, `OSS-3`) with their story points.
  - A table of **Issues not completed** (if any were remaining).

---

## 4. Verification
To verify that Practical 6 has been completed successfully:
1. Open **Spaces / Projects** -> confirm **Online Shopping Site (`OSS`)** exists.
2. In **Backlog**, confirm all 5 user stories were created and estimated with points: 3, 3, 5, 8, 13 (Total: 32).
3. In **Reports -> Sprint Report**, confirm that **OSS Sprint 1** is listed as completed with its velocity and burn-down trajectory displayed.

---

## 5. Troubleshooting
| Issue | Cause | Solution |
| :--- | :--- | :--- |
| Story Points field is missing when creating a story | Story Points field is hidden in the company screen scheme | Open the story card -> click `...` -> **Configure fields** -> check **Story Points** (or **Estimation**). |
| *"Start sprint"* button is disabled | Sprint contains 0 issues or user lacks Sprint Admin rights | Ensure at least one issue is inside the sprint container and your account has project admin permissions. |
| Cannot complete the sprint | You are viewing the Backlog instead of Active Sprints | Click **Active sprints** in the left sidebar; the **Complete sprint** button is located at the top-right of that page. |
| Reports tab is missing in sidebar | Project features toggle has Reports disabled | Go to **Space settings -> Features** -> toggle **Reports** to Enabled. |

---

## 6. Result
A Company-managed Scrum project titled **"Online Shopping Site"** (`OSS`) was successfully created. A sprint (**OSS Sprint 1**) was planned with 5 user stories totaling **32 Story Points**, started for a 2-week iteration, progressed across the board, completed, and analyzed through the generated **Sprint Report**.

---

## 7. Viva Preparation

**Q1: What is the primary difference between a Scrum board and a Kanban board?**  
*Answer:* A **Scrum board** operates on fixed-length, time-boxed iterations called sprints (usually 2 weeks) and tracks committed vs. completed work. A **Kanban board** focuses on continuous delivery and limits Work-In-Progress (WIP) without fixed sprint boundaries.

**Q2: What are Story Points, and why are Fibonacci numbers (1, 2, 3, 5, 8, 13) commonly used?**  
*Answer:* Story Points measure the relative effort and complexity of a user story rather than absolute calendar hours. Fibonacci numbers reflect increasing uncertainty as task sizes grow larger.

**Q3: What is a Burndown Chart in Jira?**  
*Answer:* A Burndown Chart shows the actual amount of work remaining in a sprint day-by-day compared to an ideal guideline burn-down rate, helping teams forecast whether sprint goals will be met.

**Q4: What happens to incomplete issues when a sprint is completed?**  
*Answer:* Jira prompts the user to either move the uncompleted issues back to the general **Product Backlog** or roll them directly into a **New / Next Sprint**.

**Q5: What is Team Velocity in Scrum?**  
*Answer:* Velocity is the average number of Story Points a Scrum team successfully completes within a sprint, used to plan future sprint capacities.

---

## 8. Practical Checklist
- [ ] Created Company-managed Scrum project `Online Shopping Site` (`OSS`).
- [ ] Opened Backlog and inspected `OSS Sprint 1`.
- [ ] Created 5 user stories (`OSS-1` through `OSS-5`).
- [ ] Assigned Story Points: 3, 3, 5, 8, 13 (Total 32 points).
- [ ] Started `OSS Sprint 1` with a 2-week duration and goal.
- [ ] Verified issues in `Active sprints` board (`TO DO` column).
- [ ] Moved issues to `IN PROGRESS` and `DONE`.
- [ ] Clicked **Complete sprint** and reviewed Summary & Sprint Reports.
