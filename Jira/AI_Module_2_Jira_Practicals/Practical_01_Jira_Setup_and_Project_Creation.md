# Practical 1: Jira Setup & Project Creation

> **Source:** AI Module 2 Lab Manual (Pages 1–7)  
> **Course:** BSc IT — Artificial Intelligence / Agile Project Management  
> **Platform:** Atlassian Jira Cloud  

---

## 1. Objective
To set up a Jira Cloud account using Google authentication, explore the default Jira workspace/dashboard, create a **Company-managed Kanban project** (named **"AI learning"** with key **"AL"**), and configure essential project settings such as project name, key, lead, and details.

---

## 2. Requirements
1. A desktop/laptop computer with a modern web browser (Google Chrome, Firefox, Safari, or Microsoft Edge).
2. A reliable internet connection.
3. An active Google (Gmail) account for Atlassian authentication.
4. Access to [https://www.atlassian.com/software/jira](https://www.atlassian.com/software/jira).
5. Administrative permissions to create a new Jira site and project (granted automatically on initial signup).

> **Note on Jira Terminology:** In some Jira Cloud editions, projects may be referred to as **"Spaces"** or **"Projects"**, depending on whether work management or software product templates are active. Both refer to the container holding your boards, tasks, and workflows.

---

## 3. Procedure

### Part A: Create a Jira Cloud Account and Explore the Dashboard
*(Refer to PDF Pages 1–4)*

#### Step 1: Search for Jira
- **Navigation:** Open Google Chrome and go to `https://www.google.com`.
- **Action:** In the search bar, type `Jira` and press **Enter**.
- **Expected result:** Google search results appear displaying the Jira Software listing by Atlassian.

#### Step 2: Open the Jira Official Website
- **Navigation:** Google Search results page.
- **Action:** Click on the official Atlassian Jira website link (`https://www.atlassian.com/software/jira`).
- **Expected result:** The Jira product homepage opens with the headline *"Where your teams and AI come together"*.

#### Step 3: Choose Google Sign-In
- **Navigation:** Jira Signup page.
- **Action:** Under the **"Or continue with"** section, click on the **Google** icon/button (`G Google`).
- **Expected result:** Google OAuth sign-in dialog or redirection screen appears.

#### Step 4: Sign in with Your Google Account
- **Navigation:** Google accounts login screen (`accounts.google.com`).
- **Action:** Enter your Gmail address, click **Next**, enter your password, and click **Next**.
- **Expected result:** Google authenticates your identity and redirects you back to Atlassian.

#### Step 5: Complete Account Creation
- **Navigation:** Atlassian *"Create your account"* screen.
- **Action:** Verify your email address and display name (e.g., `sayali birje`), then click **Continue**.
- **Expected result:** The account is confirmed and the site creation prompt is displayed.

#### Step 6: Create Your Atlassian Cloud Site
- **Navigation:** *"Create a site"* screen.
- **Action:** Enter a unique site name for your Jira Cloud domain (e.g., `birjesayali20.atlassian.net` as illustrated in the manual) and click **Continue**.
- **Expected result:** The screen displays *"Getting things ready..."* while Atlassian provisions your cloud environment.

#### Step 7: Select Your Work Category
- **Navigation:** *"What kind of work do you do?"* onboarding screen.
- **Action:** From the list of options (Software development, Marketing, IT support, etc.), select **Project management**.
- **Expected result:** Jira tailors recommended templates suited for project management.

#### Step 8: Select the Initial Kanban Template
- **Navigation:** Template suggestion screen.
- **Action:** Select **Kanban** (*"Manage and track agile work with visual columns"*) and click **Continue**.
- **Expected result:** A prompt asking you to name your space/project appears.

#### Step 9: Name Your Initial Workspace / Space
- **Navigation:** *"Name your space"* screen.
- **Action:** Enter `My First Project` in the name input field and click **Get started**.
- **Expected result:** The setup wizard configures your first workspace.

#### Step 10: Complete Onboarding and Open Jira Dashboard
- **Navigation:** *"How do you track work?"* / *"Jira's better when used together"* screen.
- **Action:** Click **Next**, then click **Go to Jira** (skip teammate invitations if prompted).
- **Expected result:** The main Jira Cloud navigation dashboard is displayed with the top navigation bar, side navigation, and your default workspace.

---

### Part B: Create a Company-Managed Kanban Project
*(Refer to PDF Pages 5–6)*

#### Step 11: Open the Project / Space Creation Menu
- **Navigation:** Top navigation bar -> Click on **Spaces** (or **Projects**).
- **Action:** From the dropdown menu, click **+ Create space** (or **Create project**).
- **Expected result:** The *"Space templates"* / *"Project templates"* catalog opens showing categories like Work management, Software development, and Service management.

#### Step 12: Select the Kanban Template
- **Navigation:** Space templates -> Categories -> **Work management** or **Software development**.
- **Action:** Locate and click on the **Kanban** card (*"Work efficiently and visualize work on a board"*).
- **Expected result:** A preview modal describing the Kanban template and its workflow statuses appears.

#### Step 13: Confirm Template Selection
- **Navigation:** Kanban template preview window.
- **Action:** Click the blue **Use template** button at the bottom right.
- **Expected result:** The *"Name your space / project"* configuration form opens.

#### Step 14: Configure Project Name and Management Type
- **Navigation:** *"Name your space"* form.
- **Action:**
  1. In the **Name** field, enter: `AI learning`
  2. The **Key** field will automatically populate as `AL` (or enter `AL` manually).
  3. Under **How your space is managed**, select: **Company-managed**.
  4. Click **Next**.
- **Expected result:** Jira creates the project architecture.

> **Clarification Note:** 
> - **Company-managed projects:** Centrally standardized projects where schemes (workflows, issue types, permissions) can be shared across multiple projects.
> - **Team-managed projects:** Isolated projects where individual teams can modify their own configurations without admin rights.

#### Step 15: Skip Teammate Invitations During Setup
- **Navigation:** *"Bring your team along"* screen.
- **Action:** Click **I'll do this later**, then click **Next** / **Done**.
- **Expected result:** Jira displays the message *"Jira space successfully created"* and redirects to your newly created Kanban board.

#### Step 16: Inspect the Kanban Board
- **Navigation:** Project dashboard -> **AL board**.
- **Action:** Observe the board structure and column layout.
- **Expected result:** The **AL board** displays four default columns:
  - `BACKLOG`
  - `SELECTED FOR DEVELOPMENT`
  - `IN PROGRESS`
  - `DONE`

---

### Part C: Configure Project Details
*(Refer to PDF Page 7)*

#### Step 17: Navigate to Project / Space Settings
- **Navigation:** On the AL board page, look at the left sidebar menu or the project drop-down menu.
- **Action:** Click on **Space settings** (or **Project settings**).
- **Expected result:** The project settings overview page opens with a sidebar containing Details, Summary, People, Permissions, Notifications, and Workflows.

#### Step 18: Review and Modify Project Details
- **Navigation:** Space settings -> **Details**.
- **Action:**
  1. **Name\*:** Verify or update the name to `AI learning`.
  2. **Space key\* / Project key\*:** Verify the key is `AL`.
  3. **URL:** View the unique web address for the project space.
  4. **Project Lead:** Confirm your account is selected as the default lead.
  5. **Icon / Avatar:** Optionally click **Change icon** to set a project image.
  6. Click **Save** (if modifications were made).
- **Expected result:** A success notification confirming project details have been saved is displayed.

---

## 4. Verification
To verify that Practical 1 has been executed successfully:
1. Open Jira and click on **Spaces** / **Projects** in the top navigation bar.
2. Verify that **AI learning (AL)** is listed under Recent/All spaces.
3. Open **AL board** and verify the 4 standard columns (`BACKLOG`, `SELECTED FOR DEVELOPMENT`, `IN PROGRESS`, `DONE`).
4. Navigate to **Space settings -> Details** and confirm:
   - Project Name: `AI learning`
   - Key: `AL`
   - Type: `Company-managed software` / `Work management`

---

## 5. Troubleshooting
| Issue | Cause | Solution |
| :--- | :--- | :--- |
| Cannot find *"Spaces"* menu | Newer Jira Cloud UI defaults to *"Projects"* | Look for **Projects** in the top navigation bar; the functionality is identical. |
| Key `AL` already in use | A previous project used the key `AL` | Enter an alternative key like `AIL` or `AILE` in the Key field. |
| Cannot select *"Company-managed"* | Free tier or certain template paths default to team-managed | In the template selection step, click **More templates** or scroll down to select **Company-managed**. |
| Google authentication loop | Third-party cookies blocked in browser | Enable third-party cookies or add `atlassian.com` to your browser's allowed sites. |

---

## 6. Result
A Jira Cloud account was successfully created and configured using Google authentication. A Company-managed Kanban project named **"AI learning"** with key **"AL"** was created, and its project details were configured and verified on the Jira dashboard.

---

## 7. Viva Preparation

**Q1: What is Atlassian Jira and what is its primary purpose?**  
*Answer:* Jira is an agile project management and issue-tracking software tool developed by Atlassian. It is widely used for bug tracking, task tracking, sprint planning, and managing agile workflows (Scrum and Kanban).

**Q2: What is the difference between a Company-managed project and a Team-managed project in Jira?**  
*Answer:* A Company-managed project is configured by Jira administrators and uses shared global configuration schemes (workflows, issue types, permission schemes) across an organization. A Team-managed project allows independent teams to customize their own boards and workflows without global admin rights.

**Q3: What is a Project Key in Jira, and why is it important?**  
*Answer:* A Project Key is a short, unique identifier (typically 2–10 uppercase letters, such as `AL`) that serves as a prefix for all issues created within that project (e.g., `AL-1`, `AL-2`).

**Q4: What is the main purpose of a Kanban board?**  
*Answer:* A Kanban board provides a continuous visual workflow using columns (e.g., Backlog, In Progress, Done) to manage work-in-progress (WIP), optimize efficiency, and identify bottlenecks.

**Q5: What are the default columns created on a Jira Kanban board?**  
*Answer:* The standard default columns are `BACKLOG`, `SELECTED FOR DEVELOPMENT`, `IN PROGRESS`, and `DONE`.

---

## 8. Practical Checklist
- [ ] Registered/signed in to Jira Cloud via Google.
- [ ] Created initial workspace site domain.
- [ ] Created Company-managed Kanban project named `AI learning`.
- [ ] Verified project key `AL`.
- [ ] Opened `AL board` and checked column layout.
- [ ] Navigated to Project/Space Settings -> Details and validated configuration.
