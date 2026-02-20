Project: “DevOps Student Portfolio Portal”
🎯 Objective

Create a single shared GitHub repository where every student contributes their profile into a collaborative project — using proper Git branching and PR workflow.

They will experience:

Real collaboration

Merge conflicts

Rebase practice

Pull request lifecycle

Code review

🏗️ Repository Structure

You (as instructor) will create a GitHub repo:

devops-git-collab-2026

Initial structure:

devops-git-collab-2026/
│
├── README.md
├── students/
│   └── README.md
├── index.html
└── contributors.md
📝 Initial Setup (You Do This)
Step 1: Create repo in GitHub

Create repo:

devops-git-collab-2026
Step 2: Add Base Files
📄 README.md

Explain project rules.

📄 contributors.md

Add one line:

# Contributors List
📄 index.html (basic template)
<!DOCTYPE html>
<html>
<head>
    <title>DevOps Git Collaboration Project</title>
</head>
<body>
    <h1>DevOps Batch - Git Collaboration Project</h1>
    <ul id="student-list">
    </ul>
</body>
</html>

Push this as main.

👨‍🎓 Student Task Overview

Each student must:

Clone the repository

Create their own feature branch

Add their profile

Update contributors list

Push branch

Raise Pull Request

Resolve conflicts if any

Get PR approved

Merge to main

📌 Detailed Task Instructions (Give to Students)

You can copy-paste this to them 👇

🧑‍💻 TASK 1 – Clone the Repository
git clone <repo-url>
cd devops-git-collab-2026
🌿 TASK 2 – Create Feature Branch

Branch naming format:

feature/<your-name>

Example:

feature/priyanka-sr
feature/ajay-kumar

Command:

git checkout -b feature/your-name
📂 TASK 3 – Create Your Profile File

Inside students/ folder create:

students/your-name.md

Example:

students/priyanka-sr.md

Content format:

# Priyanka S R

- Role: DevOps Engineer (Aspirant)
- Skills: Git, GitHub, Linux
- Learning Goal: Master CI/CD
- Fun Fact: Loves automation
📄 TASK 4 – Update contributors.md

Open contributors.md

Add your name at bottom:

- Priyanka S R

⚠️ Everyone edits same file → This WILL cause merge conflicts → That is intentional 😈

🌐 TASK 5 – Update index.html

Add your name inside <ul>:

<li>Priyanka S R</li>

Again → This will create conflicts → Good learning opportunity.

💾 TASK 6 – Commit Changes
git add .
git commit -m "Added profile for <your-name>"
🚀 TASK 7 – Push Branch
git push origin feature/your-name
🔁 TASK 8 – Create Pull Request

On GitHub:

Go to repository

Click “Compare & Pull Request”

Add proper PR title:

Add profile: Priyanka S R

Add description:

What files added

What changes made

🔥 TASK 9 – Handle Merge Conflicts (Important)

When PR shows:

"This branch has conflicts"

Students must:

git checkout feature/your-name
git pull origin main

Resolve conflict manually in:

contributors.md

index.html

Then:

git add .
git commit -m "Resolved merge conflict"
git push
🎯 Learning Outcomes

By doing this, students will understand:

Concept	Practical Exposure
git clone	Download remote repo
git checkout -b	Feature branching
git add/commit	Local version control
git push	Send code to remote
Pull Request	Collaboration workflow
Merge Conflict	Real world issue
Rebase vs Merge	Can experiment
Branch naming	Git flow discipline
💣 Advanced Challenge (Optional)

After 10 students merge:

Introduce:

🔄 Rebase Challenge

Tell remaining students:

Instead of:

git pull origin main

They must:

git fetch origin
git rebase origin/main

Then push with:

git push --force

This gives real rebase experience.

🏆 Bonus Task (Team Activity)

Divide class into 4 teams:

Team 1 – UI Enhancement

Improve index.html styling.

Team 2 – Add CSS file

Create style.css.

Team 3 – Add JavaScript

Add search filter for students.

Team 4 – Create Git Workflow Guide

Improve README with Git commands.

Each team works on:

feature/team-ui
feature/team-css
feature/team-js
feature/team-docs
💡 Instructor Strategy (Important)

To maximize chaos (learning 😎):

Merge PRs randomly

Approve some quickly

Delay some

Ask them to rebase

Reject PR with comments

Make it realistic.

🧠 Real DevOps Simulation

This simulates:

Enterprise Git workflow

Team collaboration

CI/CD merge process

Code review lifecycle

Conflict resolution under pressure
