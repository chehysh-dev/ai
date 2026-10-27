# Practical 7: Kanban Board Management

> **Source:** AI Module 2 Lab Manual (Pages 24–28)  
> **Course:** BSc IT — Artificial Intelligence / Agile Project Management  
> **Platform:** Atlassian Jira Cloud  

---

## 1. Objective
To create and configure a **Company-managed Kanban project** (**"AI Education Bot"**, Key: **`ED`** / **`AEB`**), manage work items through continuous visual delivery, configure task assignment, priority, and due dates, track task progression across Kanban workflow columns, and generate advanced agile analytical reports including the **Cumulative Flow Diagram (CFD)** and **Control Chart**.

---

## 2. Requirements
1. Jira Cloud administrative or project creation privileges.
2. An active computer with a modern browser and internet access.
3. Theoretical understanding of Kanban principles:
   - **Continuous Flow:** Work items are delivered continuously without sprint boundaries.
   - **Visualizing Workflow:** Using board columns to expose work in progress and queues.
   - **Lead Time & Cycle Time:** Measuring the time elapsed from task request to delivery.
   - **Cumulative Flow Diagram (CFD):** Visual graph tracking the volume of work in each status over time to detect process bottlenecks.

---

## 3. Procedure

### Part A: Create a Company-Managed Kanban Project
*(Refer to PDF Pages 24–26)*

#### Step 1: Open the Space / Project Creation Dialog
- **Navigation:** Top navigation bar -> Click **Spaces** (or **Projects**) -> Click **+ Create space** (or **Create project**).
- **Action:** Open the project template catalog.
- **Expected result:** The template catalog opens showing Work management, Software development, and Service management options.

#### Step 2: Select the Kanban Template
- **Navigation:** Space templates -> Categories -> Select **Software development** (or **Work management**).
- **Action:** Select the **Kanban** template (*"Work efficiently and visualize work on a board with to do, doing, and done"*).
- **Expected result:** The Kanban template overview is displayed.

#### Step 3: Click Use Template
- **Navigation:** Bottom-right corner of the template preview.
- **Action:** Click the blue **Use template** button.
- **Expected result:** The project configuration form opens.

#### Step 4: Configure Project Name and Management Type
- **Navigation:** *"Name your space"* form.
- **Action:**
  1. In the **Name\*** field, enter:
     ```text
     AI Education Bot
     ```
  2. The **Key\*** field auto-populates as `ED` or `AEB` (enter `ED` if you wish to match the manual's `ED-1` ticket key).
  3. Under **How your space is managed\***, select: **Company-managed**.
  4. Click **Next**.
- **Expected result:** The project architecture is established.

#### Step 5: Handle Teammate Invitations
- **Navigation:** *"Bring your team along"* screen.
- **Action:** Enter teammate emails (or click **I'll do this later**), then click **Next** -> **Done**.
- **Expected result:** The message *"Jira space successfully created"* appears, and the project opens directly into the **ED board** (or `AEB board`).

#### Step 6: Inspect the Kanban Board Columns
- **Navigation:** Project view -> **Kanban board**.
- **Action:** Observe the column layout.
- **Expected result:** The Kanban board displays four default visual workflow columns:
  - `BACKLOG`
  - `SELECTED FOR DEVELOPMENT`
  - `IN PROGRESS`
  - `DONE`

---

### Part B: Create and Configure a Kanban Task
*(Refer to PDF Pages 26–27)*

#### Step 7: Create a New Task in Backlog
- **Navigation:** Under the **BACKLOG** column on the Kanban board.
- **Action:** Click the **+ Create** button (or click the top navigation **+ Create** button).
- **Expected result:** The inline creation card appears with the prompt *"What needs to be done?"*.

#### Step 8: Enter the Task Title and Issue Type
- **Navigation:** Inline text box.
- **Action:**
  1. Type the task summary:
     ```text
     Create user registration and login system
     ```
  2. In the issue type dropdown, verify that **Task** (`🟦 Task`) is selected.
  3. Press **Enter**.
- **Expected result:** The task is created with key **`ED-1`** (or `AEB-1`) and card title *"Create user registration and login system"* in the **BACKLOG** column.

#### Step 9: Assign the Task to a Team Member
- **Navigation:** On the **`ED-1`** card face -> Locate the circular **Unassigned** user icon (gray circle with silhouette).
- **Action:** Click the icon to open the quick-assign dropdown menu. Select a team member (e.g., `Sayali Birje (Assign to me)`, `marry.rose`, or `john.smith`).
- **Expected result:** The assignee icon immediately updates to display the assigned user's avatar.

#### Step 10: Set Task Priority and Due Date
- **Navigation:** Click on the **`ED-1`** card to open the issue details panel.
- **Action:**
  1. In the **Priority** field, select **High** or **Highest**.
  2. In the **Due date** field, select a completion deadline from the calendar picker.
  3. Close the details panel.
- **Expected result:** The card face on the board displays the updated priority icon and scheduled due date.

#### Step 11: Progress the Task Through Kanban Workflow Columns
- **Navigation:** Kanban board columns.
- **Action:** Drag and drop the **`ED-1`** card across columns as work proceeds:
  1. Drag from `BACKLOG` -> `SELECTED FOR DEVELOPMENT`.
  2. Drag from `SELECTED FOR DEVELOPMENT` -> `IN PROGRESS`.
  3. When development and testing are finished, drag from `IN PROGRESS` -> `DONE`.
- **Expected result:** The card smoothly transitions between states, reflecting real-time workflow status.

---

### Part C: Track Issue Progress and Generate Agile Reports
*(Refer to PDF Page 28)*

#### Step 12: Navigate to Project Reports
- **Navigation:** Left sidebar menu -> Click on **Reports**.
- **Action:** Review the default reporting dashboard or click on **More reports** (or **Agile reports**).
- **Expected result:** The Reports catalog displays analytical tools grouped into categories: *Agile*, *Issue analysis*, and *Forecast & management*.

#### Step 13: Generate Cumulative Flow Diagram (CFD)
- **Navigation:** Reports catalog -> Under **Agile** section.
- **Action:** Click on **Cumulative Flow Diagram**.
- **Expected result:** The Cumulative Flow Diagram renders:
  - **X-axis:** Timeline (dates).
  - **Y-axis:** Cumulative number of issues.
  - **Colored bands:** Area bands showing the volume of issues in each status (`Backlog`, `Selected for Development`, `In Progress`, `Done`).
  - **Analysis:** Horizontal distance between bands indicates Cycle Time; widening bands indicate accumulation of bottlenecked work.

#### Step 14: Inspect the Control Chart
- **Navigation:** Reports -> Agile -> Click on **Control Chart**.
- **Action:** Examine the chart data points and curves.
- **Expected result:** The Control Chart renders:
  - Individual data points representing completed issues.
  - The **Rolling Average** line showing mean cycle time.
  - The **Standard Deviation (shaded band)** showing process stability and predictability.

---

## 4. Key Differences: Cumulative Flow Diagram vs. Control Chart

| Feature | Cumulative Flow Diagram (CFD) | Control Chart |
| :--- | :--- | :--- |
| **Primary Metric** | Work-In-Progress (WIP) and Bottlenecks | Cycle Time and Process Lead Time |
| **Visual Appearance** | Multi-colored stacked area chart | Scatter plot of issues with rolling average trend lines |
| **Key Insight** | Parallel bands indicate healthy flow; expanding bands reveal bottlenecks | Clustered points near the average mean indicate a stable, predictable delivery process |
| **Agile Value** | Helps optimize throughput and WIP limits | Helps forecast realistic customer delivery dates |

---

## 5. Verification
To verify that Practical 7 has been executed successfully:
1. Open **Spaces / Projects** -> Verify **AI Education Bot (`ED` / `AEB`)** is listed.
2. On the **Kanban board**, verify that issue **`ED-1: Create user registration and login system`** exists, is assigned, and transitioned to `DONE`.
3. In **Reports -> Cumulative Flow Diagram**, confirm that the graph renders data reflecting the status transition history of `ED-1`.

---

## 6. Troubleshooting
| Issue | Cause | Solution |
| :--- | :--- | :--- |
| CFD shows flat lines or no data | Issue was created and completed on the same minute | CFD aggregates daily status snapshots; data points will be fully visible after 24–48 hours of board activity or by zooming into the timeframe filter. |
| Cannot drag card to *"Done"* column | Column transition is restricted by workflow rule | Ensure the user dragging the card is assigned to the issue or holds project administrator permissions. |
| *"Reports"* link missing from sidebar | Reports feature disabled in space settings | Navigate to **Space settings -> Features** and toggle **Reports** to Enabled. |
| WIP Limit warning displayed on column | A column has exceeded its configured Work-In-Progress limit | This is normal Kanban behavior to alert teams of overload; move existing items to Done before pulling new tasks. |

---

## 7. Result
A Company-managed Kanban project named **"AI Education Bot"** (`ED`) was successfully created. A development task (`ED-1`) was configured, assigned, scheduled, and progressed through the Kanban visual workflow columns. Process analytics were evaluated using the **Cumulative Flow Diagram** and **Control Chart**.

---

## 8. Viva Preparation

**Q1: What is the core philosophy behind Kanban?**  
*Answer:* Kanban focuses on visualizing work, limiting Work-In-Progress (WIP) at each stage, maximizing process efficiency, and achieving continuous delivery without fixed sprint deadlines.

**Q2: What is Work-In-Progress (WIP) and why is it limited in Kanban?**  
*Answer:* WIP is the number of active tasks currently being worked on between Backlog and Done. Limiting WIP prevents multitasking, reduces cycle time, and prevents team burnout.

**Q3: What does the Cumulative Flow Diagram (CFD) tell an agile team?**  
*Answer:* The CFD visualizes the number of issues in each state over time. Parallel bands represent consistent throughput, while a widening band indicates that work is accumulating and a bottleneck exists at that stage.

**Q4: What is the difference between Lead Time and Cycle Time?**  
*Answer:* **Lead Time** is the total time from when a customer requests a task until it is delivered. **Cycle Time** is the time spent actively working on the task from the moment work begins until completion.

**Q5: What does the Control Chart display in Jira?**  
*Answer:* The Control Chart plots the cycle time of individual issues along with a rolling average and standard deviation, helping teams measure consistency and forecast future performance.

---

## 9. Practical Checklist
- [ ] Created Company-managed Kanban project `AI Education Bot` (`ED`).
- [ ] Verified the four default Kanban columns.
- [ ] Created task `Create user registration and login system` (`ED-1`).
- [ ] Assigned task to an active project team member.
- [ ] Configured Priority and Due Date.
- [ ] Progressed card through `Selected for Development`, `In Progress`, and `Done`.
- [ ] Opened Reports -> More reports -> Cumulative Flow Diagram.
- [ ] Inspected the Control Chart and analyzed cycle time metrics.
