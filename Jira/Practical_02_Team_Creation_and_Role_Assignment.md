# Practical 2: Team Creation and Role Assignment

> **Source:** AI Module 2 Lab Manual (Pages 8–9)  
> **Course:** BSc IT — Artificial Intelligence / Agile Project Management  
> **Platform:** Atlassian Jira Cloud  

---

## 1. Objective
To invite and add team members to an existing Jira project (**"AI learning"** / **"AL board"**), assign appropriate project roles (e.g., Administrator, Member, Viewer), and inspect team member permissions within project settings.

---

## 2. Requirements
1. Access to the Jira Cloud instance configured in Practical 1.
2. Administrator or project management permissions to invite users to the project/space.
3. At least one valid email address of a teammate, peer, or secondary student account to send an invitation.
4. A web browser connected to the internet.

> **Important Note on User Licences & Privacy:** 
> - Do not invent arbitrary fictional email addresses that you do not control. For practical examinations, use your own secondary email or a partner student's email.
> - In Jira Cloud Free tier, adding users consumes one of your 10 free user licences.

---

## 3. Procedure

### Part A: Access the Project Board
*(Refer to PDF Page 8)*

#### Step 1: Open the Existing Project Board
- **Navigation:** Open Jira Cloud -> Top navigation -> Click **Spaces** (or **Projects**) -> Select **AI learning** -> Open **AL board**.
- **Action:** Wait for the Kanban board to load completely.
- **Expected result:** The **AL board** is displayed showing the active Kanban columns (`BACKLOG`, `SELECTED FOR DEVELOPMENT`, `IN PROGRESS`, `DONE`).

#### Step 2: Locate the "Add People" Option
- **Navigation:** Top-left header section of the board, next to the board title or via the top navigation bar.
- **Action:** Click on the **Add people** button (or the user profile icon with a plus `+` symbol).
- **Expected result:** The *"Add people to AI learning"* dialog modal opens over the board.

---

### Part B: Invite Team Members and Assign Roles
*(Refer to PDF Page 9)*

#### Step 3: Enter the Team Member's Email Address
- **Navigation:** *"Add people to AI learning"* dialog.
- **Action:** Click on the **Names or emails\*** text field and type the email address of the team member (for example: `sayali.birje@avc.ac.in` as shown in the lab demonstration, or your lab partner's email).
- **Expected result:** The typed email address is validated and displayed as a selectable token.

#### Step 4: Assign a Project Role
- **Navigation:** *"Role\*"* dropdown menu inside the dialog.
- **Action:** Click the **Role** dropdown and select the desired permission role:
  - **Administrator:** Full administrative control over the project settings, components, versions, and boards.
  - **Member (Default):** Standard team member role capable of creating, editing, and moving issues across board columns.
  - **Viewer:** Read-only access to view issues and boards without edit permissions.
- **Expected result:** The chosen role is assigned to the pending invitee.

> **Additional Integrations Note:** Notice the options underneath to import contacts directly from **Google**, **Slack**, or **Microsoft** accounts if organizational directories are linked.

#### Step 5: Send the Invitation
- **Navigation:** Bottom-right corner of the *"Add people"* dialog.
- **Action:** Click the blue **Add 1 Person** (or **Add**) button.
- **Expected result:** Jira processes the invitation, sends an automated email invitation to the recipient, and displays a confirmation dialog.

#### Step 6: Review the Confirmation Dialog
- **Navigation:** Confirmation popup box: *"Added people to space"*.
- **Action:** Read the message: *"You have added 1 person to your space and 1 new licence has been added to Jira. You can manage access from the space settings."* Then click **OK**.
- **Expected result:** The modal closes and you return to the active Kanban board.

#### Step 7: Add Additional Team Members (Repeatable)
- **Navigation:** Board header -> **Add people**.
- **Action:** Repeat Steps 3 through 6 for any additional team members (e.g., student lab partners, `john.smith`, `marry.rose`).
- **Expected result:** Each team member is invited and added to the project workspace.

---

### Part C: Inspect and Manage Project Roles & Permissions
*(Refer to PDF Page 9 & Space Settings)*

#### Step 8: Open Space / Project People Settings
- **Navigation:** Left sidebar menu -> Click **Space settings** (or **Project settings**) -> Click **People**.
- **Action:** Review the list of users associated with the **AI learning** project.
- **Expected result:** A table listing all project members, their email addresses, account status, and assigned project roles is displayed.

#### Step 9: Modify or Remove a User Role (Optional)
- **Navigation:** Space settings -> **People** tab.
- **Action:** Locate a user, click the **Role** dropdown next to their name to switch between *Administrator*, *Member*, or *Viewer*, or click the three dots (`...`) to remove them from the project.
- **Expected result:** User permissions are updated immediately without affecting other projects.

---

## 4. Understanding Jira Roles vs. Permissions

| Permission Level | Scope | Description |
| :--- | :--- | :--- |
| **Project Role** | Project-Specific | Defines what a user can do inside a specific project (e.g., *Administrator*, *Member*, *Viewer*). Assigned by the Project Admin. |
| **Group / Workspace Role** | Site-Wide | Groups like `jira-software-users` or `site-admins` determining product licence access across the entire Atlassian site. |
| **Global Permission** | System-Wide | System administrator permissions to create sites, install marketplace apps, and manage billing. |

---

## 5. Verification
To verify that Practical 2 has been completed successfully:
1. Open **AL board** and observe the top-right header: The avatar initials of the added member(s) should appear.
2. Go to **Space settings -> People**:
   - Confirm that the invited email address (e.g., `sayali.birje@avc.ac.in`) appears in the members table.
   - Confirm that their assigned role (e.g., `Member` or `Administrator`) is correctly displayed.
3. Check the invitee's inbox: An invitation email with a link to join the Jira workspace will have been received.

---

## 6. Troubleshooting
| Issue | Cause | Solution |
| :--- | :--- | :--- |
| *"You have reached your user limit"* | Free plan is capped at 10 users | Remove unnecessary inactive users via `admin.atlassian.com -> Users` or stay under 10 members. |
| Cannot see the *"Add people"* button | Insufficient project permissions | Ensure your account is logged in as the Site Administrator or Project Lead. |
| Role dropdown does not appear | Team-managed project instead of Company-managed | In team-managed projects, roles are managed via Project Settings -> Access. Follow Company-managed steps. |
| Invitee did not receive the email | Invitation caught in spam/junk filter | Ask the recipient to check their spam folder or copy the direct invitation link from Jira. |

---

## 7. Result
Team members were successfully added to the **AI learning** project via email invitation, assigned specific project roles (*Member / Administrator*), and verified in the Project People settings.

---

## 8. Viva Preparation

**Q1: What is a Project Role in Jira?**  
*Answer:* A Project Role is a flexible way to associate users and groups with specific functions in a project (such as Administrators, Developers, Members, and Viewers). Unlike global groups, project roles can have different members in different projects.

**Q2: What is the difference between a Jira User and a Jira Administrator?**  
*Answer:* A Jira User can view, create, edit, and transition issues according to project permissions. A Jira Administrator can configure project settings, customize workflows, add users, assign roles, and manage system schemes.

**Q3: Where can a project administrator view and manage all team members in a project?**  
*Answer:* Under **Project settings** (or **Space settings**) -> **People** (or **Access**).

**Q4: Can a user have different roles in different Jira projects?**  
*Answer:* Yes. Because Project Roles are project-specific, a user can be an *Administrator* in Project A while only being a *Viewer* or *Member* in Project B.

**Q5: What happens when an invited team member clicks the email invitation link?**  
*Answer:* They are prompted to log in or create an Atlassian account, after which they gain immediate access to the project board with their pre-assigned role.

---

## 9. Practical Checklist
- [ ] Opened `AL board` in the `AI learning` project.
- [ ] Clicked **Add people** button.
- [ ] Entered a valid teammate email address.
- [ ] Selected the appropriate project role.
- [ ] Verified the *"Added people to space"* confirmation message.
- [ ] Opened Space settings -> People and verified the team roster.
