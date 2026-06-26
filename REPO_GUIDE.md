# 📘 Repository Guide — How This Repo Works

> This guide explains the structure, setup, and workflow of the **My_Awards** repository.
> It is intended as a reference for future you (or collaborators) to understand how to maintain and expand this repo.

---

## 📂 Folder Structure

```
My_Awards/
│
├── README.md                          ← Main display file (rendered on GitHub)
├── .gitignore                         ← Files/folders Git should ignore
├── REPO_GUIDE.md                      ← This file (setup & workflow docs)
│
├── Outstanding President & Secretary Duo of RcSVIT 2024-25/
│   ├── Receiving_Outstanding_President...Award.jpg
│   ├── All_Awards.jpg
│   ├── With_My_Team.jpg
│   └── ...
│
├── 2nd Place in Mini Project 2024-25/
│   └── Receiving_MiniProject_Award_From_HOD.jpg
│
├── Dept technical From student coordinator 2023-24/
│   ├── department_technical_forum...Award (2023-2024).jpg
│   └── Receiving_dept_tech_forum...Award_From_Prinicple.jpg
│
├── Rotaract Awards 2024-25/
│   ├── Beach Clean Up drive kundapura 2024-2025 Award/
│   ├── Emerging Club RcSVIT form Q1 to Q4 2024-2025/
│   ├── Membership Champion of RcSVIT 2024-25/
│   ├── Promising Year Theme of RcSVIT 2024-25/
│   ├── Short Film Constant winner of Rcsvit 2024-25/
│   ├── Transformative Growth of the year of RcSVIT 2024-25/
│   └── (loose photos: 1726055388754.jpg, etc.)
│   └── MP4_20240610_150305VLOG.mp4
│
└── (future award folders go here)
```

---

## 🏗️ How This Repo Was Set Up (First Time)

### Step 1: Created a new GitHub repo
- Go to **github.com → New Repository**
- Name: `My_Awards`
- Description: `🏅 A curated showcase of my awards, recognitions, and honors`
- Visibility: **Public**
- ❌ Do NOT initialize with README (we already have one locally)

### Step 2: Initialized Git locally
```bash
cd "C:\Users\thrin\Desktop\github doc\Awards"
git init
git add .
git commit -m "🏅 Initial commit - Added 10 awards with categorized README"
```

### Step 3: Connected to GitHub & pushed
```bash
git branch -M main
git remote add origin https://github.com/thrinadh2164/My_Awards.git
git push -u origin main
```

---

## ➕ How to Add New Awards in the Future

### Step 1: Add the award folder
Create a new folder inside the `Awards` directory with a descriptive name:
```
Example: "Best Innovator Award 2025-26"
```
Place all related images (certificate scans, receiving photos, team photos) inside it.

### Step 2: Update the README.md
Open `README.md` and add the new award to the **correct category table**:

**Pick the right category:**
| Category | When to use |
|---|---|
| 🎖️ Leadership & Service Awards | Club roles, president/secretary awards, organizational honors |
| 🎓 Academic & Technical Awards | University awards, project wins, technical coordinator roles |
| 🎬 Creative & Competition Awards | Contests, hackathons, creative wins |
| 🌍 Community Service Awards | Volunteering, social drives, community impact recognitions |

**Add a row to the table:**
```markdown
| 3 | **New Award Name** | Organization Name | 2025–2026 |
```

**Add images inside the `<details>` block:**
```markdown
| Photo Description |
|:---:|
| <img src="Folder Name/image_file.jpg" width="400"/> |
```

### Step 3: Update the Summary table
At the bottom of `README.md`, update the count for the relevant category and the total.

### Step 4: Commit & Push
```bash
cd "C:\Users\thrin\Desktop\github doc\Awards"
git add .
git commit -m "🏅 Added: [Award Name] - [Category]"
git push
```

**Example commit messages:**
- `🏅 Added: Best Innovator Award 2025-26 - Academic & Technical`
- `🏅 Added: District Conference Leadership Award - Leadership & Service`
- `🏅 Added: Hackathon Winner Certificate - Creative & Competition`

---

## 🔄 Common Git Commands Reference

| Task | Command |
|---|---|
| Check what's changed | `git status` |
| Add all new files | `git add .` |
| Add specific file/folder | `git add "Folder Name/"` |
| Commit changes | `git commit -m "your message"` |
| Push to GitHub | `git push` |
| Pull latest from GitHub | `git pull` |
| See commit history | `git log --oneline -5` |
| Check remote URL | `git remote -v` |

---

## 📋 Naming Conventions

### Folder Names
- Use the **full award name** as folder name
- Include the **year** at the end
- Example: `Best Innovator Award 2025-26`

### Image Files
- Use **descriptive names** with underscores
- Include context like `Receiving_`, `With_`, `Certificate_`
- Examples:
  - `Receiving_Best_Innovator_Award.jpg`
  - `Certificate_Best_Innovator_2025-26.jpg`
  - `With_My_Team.jpg`

---

## 🔗 Related Repositories

| Repository | Description | Link |
|---|---|---|
| **My_Certifications** | Professional certifications & course completions | [View Repo](https://github.com/thrinadh2164/My_Certifications) |
| **My_Awards** | Awards, recognitions & honors (this repo) | [View Repo](https://github.com/thrinadh2164/My_Awards) |

---

## 💡 Pro Tips

1. **Keep images under 10MB each** — GitHub has a 100MB file size limit. Compress large photos before adding.
2. **Use `.jpg` or `.png`** — These render nicely in GitHub README previews.
3. **Avoid video files when possible** — Large `.mp4` files eat up your repo size. Consider uploading videos to YouTube and linking instead.
4. **Commit often** — Don't wait to accumulate many awards. Push each one as you get it.
5. **Pin this repo** — Go to your GitHub profile and pin `My_Awards` alongside `My_Certifications` for maximum visibility.

---

> 📅 **Last Updated:** June 2026
> 
> 🛠️ **Maintained by:** E Thrinadh Chowdary
