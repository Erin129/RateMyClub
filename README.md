# RateMyClub
## Members

Julio Arboleda, Erin Hargrave, Natalie Poche, Graciela Strand

## Table of Contents

- [Mission Statement](#mission-statement)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Stretch Goals](#stretch-goals)

## Mission Statement

Our project’s challenge is incoming college students struggling to find a club that matches their criteria. They often find themselves overwhelmed with the options or unable to determine what differentiates the various clubs on campus. Our application will be a resource that addresses this concern. Students will be able to observe authentic statements from current students describing their clubs and giving honest feedback, and then make educated decisions about the type of club they'd like to join. This is a problem every incoming freshman faces and can have a big impact on the rest of their college experience. Through our interface, we aim to provide valuable insight into club experiences and help struggling college students find the club best suited for them.

## Installation

### Prerequisites

Before beginning with the Installation steps, ensure that the following requirements have been met:

- You have installed Python 3.x on your system. This is for backend development.
- You have installed [Node.js](https://nodejs.org/). This is for frontend development.
- You have installed the package managers 'pip' and 'npm', which will be installed via Python or Node.js, respectively.
- All of the previous requirements are updated to the latest versions.
- Forked the repository "https://github.com/treeofjuly/ratemyclub.git"

### Installation

Follow the steps to install the project onto your system with your own branch.

1. **Clone the repository**
   - Use the following command:
     ```bash
     git clone https://github.com/treeofjuly/ratemyclub.git
     cd ratemyclub
     ```
2. **Add your Github remote repository**
   - Use the following command to see the available remote repository that Git is connected to:
     ```bash
     git remote -v
     ```
     - If done correctly, you should see a remote repository called origin or master, and its link is to the cloned Github.
   - The next step is optional and only depends on your personal preference, change the name of the remote repository "origin/master" to "upstream" to avoid confusion between the roles of the repository. Use the following command:
     ```bash
     git remote rename 'repo-name' 'new-repo-name'
     ```
   - The next step is to change the URL of your GitHub forked repository to point to your own remote repository. You can do this using the following command:
     ```bash
     git remote set-url <remote_name> <new_url>
     ```
     - After running the command you will see two remote repositories configured, meaning you will have authorization to the both of them.
3. **Creating and then switching to personal branch for contribution**
   - Use the following command to check to see if your branch exists in Github (meaning you made the branch in Github.com and not using Git in cmdline):
     ```bash
     git branch
     ```
     This should label all existing branches, and there should exist an asterisk next to a branch. This asterisk represents the branch the repository you are currently on.
   - If your branch is found then switch over using the following code:
     ```bash
     git checkout your-personal-branch
     ```
   - If your branch was not found then create your own branch and switch over using the following code:
     ```bash
     git checkout -b your-personal-branch
     ```
4. **Recreating the necessary environment for both back-end and front-end**
   - Use the following commands to set up your environment, specifically the .venv for back-end and the node_modules/ for front-end:
     ```bash
     # For backend
     cd back-end
     python -m venv .venv
     .venv/Scripts/activate
     pip install -r requirements.txt
     # After installment
     deactivate
     # For frontend
     cd .
     cd front-end
     npm install
     # To run application
     npm start
     ```
   - You are done setting it up. Back-end users must activate the .venv if to run applications
5. **Push Your Files to Finalize your Personal Branch**
   - It is time to finalize your branch by pushing your branch onto the remote repository! Use the following command:
     ```bash
     git add .
     git commit -m "Your message!"
     git push -u forked-repo-name your-personal-branch
     ```
## Usage

The following commands will be to run the front-end or back-end scripts:
```bash
npm start

python app.py
```

## Features

1. User login/authentification.
2. Creating and Editing user profiles.
3. Home page that displays a list of clubs.
4. Search and filter capabilities.
5. Unique club pages for each club.
6. Student page to view past submitted club reviews.
7. Display of average overall ratings for each club.
8. Displays a list of student reviews.
9. Thumbs up and flagging functionality.
10. Form to submit new student reviews.
11. Different page views for students, club presidents, and admin.

## Stretch Goals

Components that could be  implemented in further development:
   1. Expanding the club directory to include a larger/complete percentage of UF clubs.
   2. Creating a form to request the addition of a new club to the directory.
   3. Including a page in admin view that lists all flagged reviews for revision and easier access.
   4. Expanding the site to more universities.
   5. Adding an alphabet  scroll bar on the side.
   6. Allowing students to ‘bookmark’/save clubs and view on a separate page.
