# University Student Clubs Portal

A modern, fully responsive web platform connecting students with university clubs and campus activities.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Team Members](#team-members)
- [Folder Structure](#folder-structure)
- [Pages](#pages)
- [How to Run Locally](#how-to-run-locally)
- [Git Workflow](#git-workflow)

---

## Project Overview

The University Student Clubs Portal is a comprehensive platform designed for students to explore, join, and participate in various university clubs. The portal serves as a central hub for club information, event announcements, and community engagement. Through this platform, students can discover clubs aligned with their interests—whether in technology, sports, culture, or debate—and connect with like-minded peers to build lasting friendships and develop valuable skills.

---

## Team Members

| Sr# | Name           | Role         | Branch | Page            |
| --- | -------------- | ------------ | ------ | --------------- |
| 1   | Student Name 1 | Project Lead | CS     | Home Page       |
| 2   | Student Name 2 | Developer    | CS     | Clubs Page      |
| 3   | Student Name 3 | Developer    | SE     | Events Page     |
| 4   | Student Name 4 | Designer     | CE     | Join Page       |
| 5   | Student Name 5 | Developer    | EE     | Highlights Page |

---

## Folder Structure

```
student-portfolio/
├── .gitignore
├── README.md
├── src/
│   ├── index.html        (Home Page - Main Landing Page)
│   ├── clubs.html        (Clubs Listing Page)
│   ├── events.html       (Events Page)
│   ├── join.html         (Join Club Page)
│   └── highlights.html   (Highlights Page)
└── styles/
    └── style.css         (Central Stylesheet)
```

---

## Pages

| File                  | Page Name     | Description                                                                                               |
| --------------------- | ------------- | --------------------------------------------------------------------------------------------------------- |
| `src/index.html`      | Home Page     | Main landing page featuring hero section, stats bar, club categories, upcoming events, and call-to-action |
| `src/clubs.html`      | Clubs Listing | Browse and filter all available university clubs by category                                              |
| `src/events.html`     | Events Page   | View upcoming club events with dates, times, and registration details                                     |
| `src/join.html`       | Join Club     | Form and guide for students to join their preferred clubs                                                 |
| `src/highlights.html` | Highlights    | Showcase of achievements, success stories, and memorable club moments                                     |

---

## How to Run Locally

1. **Download/Clone the Repository**: Download the project folder to your local machine
2. **Open in Browser**: Navigate to the `src/` folder and double-click `index.html` to open in your default browser
3. **Or use a Local Server**: For better functionality, use a local server:
   - Install [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension in VS Code
   - Right-click on `src/index.html` and select "Open with Live Server"
4. **Navigate the Site**: Use the navigation menu to explore different pages and sections

---

## Git Workflow

The project follows a structured Git workflow for version control and collaboration:

```
Feature Branches → Pull Requests → Develop → Release → Main
```

### Workflow Steps:

1. **Feature Branch**: Create a feature branch from `develop` for each new feature or fix
   - Naming convention: `feature/page-name` or `fix/issue-name`
   - Example: `feature/clubs-page` or `fix/responsive-nav`

2. **Commit & Push**: Make commits with clear, descriptive messages
   - Example: `Add clubs listing cards with filter functionality`

3. **Pull Requests**: Open a PR to `develop` for code review and testing

4. **Code Review**: Team members review and approve changes

5. **Merge to Develop**: After approval, merge the feature branch into `develop`

6. **Release Branch**: When ready for release, create a `release/v1.0` branch from `develop`

7. **Testing & Fixes**: Test thoroughly and fix any issues on the release branch

8. **Merge to Main**: Merge the release branch into `main` for production

9. **Tag Release**: Create a version tag on `main` (e.g., `v1.0`)

10. **Merge Back**: Merge the release branch back into `develop`

### Example Commands:

```bash
# Start a new feature
git checkout -b feature/clubs-page develop

# Commit changes
git add .
git commit -m "Add clubs listing with search functionality"

# Push to remote
git push origin feature/clubs-page

# After PR approval, merge to develop
git checkout develop
git merge feature/clubs-page

# Create release branch
git checkout -b release/v1.0 develop

# Merge to main
git checkout main
git merge release/v1.0
git tag -a v1.0 -m "Release version 1.0"

# Merge back to develop
git checkout develop
git merge release/v1.0
```

---

**Last Updated**: March 2026 | **Version**: 1.0.0
