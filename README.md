# student repo

The repo for students taking the stand-alone Web Development course.

## Overview

The purpose of this repository is to hold a student's code solutions for exercises and challenges. It is designed to be used in a development environment on the student's personal workstation. It assumes the student will be using [VS Code](https://code.visualstudio.com/) with a Linux-like terminal, such as [ZShell](https://wiki.zshell.dev/) (standard on MacOS), [Bash](https://www.gnu.org/software/bash/) (Linux), or [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/). It also assumes students will use GitHub for their exercise solutions.

To begin, the instructor should provide instructions on cloning the `teach-student-template` repo.

## Environment Setup

The the student should set up their development environment with the tools necessary for development. The Guide [Full Stack Development Environments](./guides/Post-Program_Development-Environment/README.md) has details on setting up most of these tools. The instructor can provide detailed assistance, if necessary, to ensure these are all properly installed and configured.

The following tools are required for this class:

- [VS Code](https://code.visualstudio.com/) with the LearningFuze Extension Pack (learningfuze.lfz-pack) installed.
- A Linux-like terminal (e.g., [ZShell](https://wiki.zshell.dev/), [Bash](https://www.gnu.org/software/bash/), [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/))
- [Google Chrome](https://www.google.com/chrome/)
- [Node and NPM](https://nodejs.org)
  - Optional: Use [NVM](https://github.com/nvm-sh/nvm) for installing and managing Node and NPM versions
- [git](https://git-scm.com/) and a [GitHub](https://github.com/) account for version control. `git` is installed with Node. The student must create a `GitHub` account and set up SSH.
- [PostgreSQL](https://www.postgresql.org/) database management system. Unfortunately, this can be a challenge to set up. On Mac, a simple but effective tool is the [Postgres app](https://postgresapp.com).

In addition, the course uses various linting and code formatting tools to simplify instruction. These tools are commonly used in the industry, and the rules that are applied in this course are similar to those used at many companies. Those tools are:

- [Prettier](https://prettier.io/) for formatting code. It is strongly suggested that students select Prettier as the Default Formatter and enable "Format on Save" in their VS Code settings.
- [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig) for additional formatting rules.
- [ESLint](https://eslint.org/) for linting (finding bugs) in TypeScript code.
- [StyleLint](https://stylelint.io/) for linting (finding bugs) in CSS.
- [MarkupLint](https://markuplint.dev/) for linting (finding bugs) in HTML.

These linting and formatting tools are all installed in the root `package.json` and/or enabled in the LearningFuze Extensions Pack.

### Student Solution Repo

The student should create a repo in GitHub to hold all the exercise solutions. This is done by navigating to the [`teach-student-template`](https://github.com/RobertGardner/teach-student-template) repo and clicking the "Use this template" button. (Note, the student must be signed in to GitHub.) The solution repo can have any name.

The instructor should share the `Guides.zip` with the student using an appropriate mechanism. The student must then unzip the file and copy the `guides` folder into their VS Code solution repo, at the root of the repo. Within VS Code, the `guides` folder can now be opened to see all the Guides. A Guide can be viewed by opening the Guide folder, right-clicking `README.md` and choosing "Open Preview".

## Instruction

The Web Development course consists of two Parts:

- Part 1 - Frontend Development with TypeScript, HTML, CSS
- Part 2 - Full Stack Development with React, Node/Express, PostgreSQL

Part 1 focuses on learning fundamental programming skills. It covers the TypeScript programming language, HTML & CSS, and manipulating the DOM using TypeScript.

Part 2 focuses on using fundamental skills to build full stack projects using frameworks, servers, and databases. It uses the **PERN** stack (**P**ostgreSQL, **E**xpress, **R**eact, and **N**ode). The choice of stack is not important. Learning the concepts of full stack software development _is_ important. However, the PERN stack uses frameworks and infrastructure that is very popular in the industry.

The course material uses a [flipped classroom](https://en.wikipedia.org/wiki/Flipped_classroom) teaching style. With this teaching style, the day flows as follows:

- Instructor assigns an exercise.
- Student reads the exercise instructions in the `README` file, browses material referenced in the exercise, completes the exercise steps, and answers any quiz questions in the accompanying `quiz-notes.md` file.
- Once completed, the student commits the exercise on a branch, pushes it to GitHub, creates a PR, and sends the PR link to the instructor.
- Once the students (or a large percentage of the students) are finished, the instructor reviews the PRs and begins a "Q&A" session.
- In the Q&A session, the instructor asks the students each question, discusses it, and works through the exercise so the students can see how a professional developer would approach the problem.
- Repeat! Typically, 2-4 exercises are covered each 8 hour day.

There are several different types of exercises and activities covered in the curriculum:

- Exercise
- Challenge
- Project
- Hack-a-thon
- Final Project

An **Exercise** contains step-by-step instructions that the student carries out to practice or learn different programming techniques.

A **Challenge** provides a spec that the student must recreate, without step-by-step instructions. These give the student the opportunity to solidify what they have learned and see how it all fits together. Challenges are delivered to students in the same way as exercises. They are distinguished from exercises by using the word "Challenge" in the exercise instructions.

A **Project** is a large, often multi-day project that is implemented in a separate repo that is not part of the code solutions repo. Projects instructions are in the Guides, in the "Project Instructions" section. They usually have a separate template repo that students can use to get started.

A **Hack-a-thon** is a multi-person project. They last for one day with the students working together to complete the work. Students take turns writing code for the project. At the end of the allotted time, the team's work is submitted, in whatever state it is in. Students are not expected to complete unfinished hack-a-thon projects.

A **Final Project** is a project that the student chooses, designs, and implements on their own. There is a final project at the end of each class Part. They typically take 1-3 weeks to complete. Experience has shown that these projects are where the bulk of the student learning takes part. They give students the opportunity to pull together everything they have learned, make mistakes, ask questions, and internalize the skills they have learned. These projects are critical for student learning.

### Starting an Exercise

The exercise materials will be distributed using an appropriate file sharing tool as a zip file. The student should unzip the file (for example, by double-clicking it) and drag the resulting folder into their solution repo, at the root of the repo. This can be done by dragging the file directly into the repo file system, or by dragging the file into the VS Code Explorer panel.

The exercise folder will contain all the materials necessary for completing the exercise. Included in the materials will be a folder named `instructions`, which contains the instructions for the exercise.

The student can read the exercise instructions by opening the exercise folder in VS Code, then opening the `instructions` folder, and finally right-clicking `README.md` and choosing "Open Preview". The original `README.md` tab can then be closed. If it is easier to have the instructions in a separate window, open the file in VS Code, then right-click the `README.md` tab and choose "Move into New Window". In the new window, open the preview.

Before starting work on an exercise, create a `git` branch for the exercise solution. A branch can be easily created in VS Code either by choosing "Branch > Create Branch..." in the Source Control panel, or by clicking the branch name in the lower-left corner of the VS Code window. While the name of the branch can be arbitrary, it is recommended that the branch name match the exercise name.

After reading all the material, the student should carry out the instructions in the "Exercise" portion of the README, by creating or editing files in the exercise folder.

Each exercise contains a file named `EXERCISE-NAME-quiz-notes.md` (or just `EXERCISE-NAME-notes.md` if there are no quiz questions). The student should use this file to record any notes they want to remember about the exercise and/or to capture their answers to the quiz questions. This file will be submitted to GitHub as part of the exercise PR.

Details can be found in the [Starting an Exercise Guide](./guides/Exercise-Workflow_Starting-an-Exercise/README.md).

### Submitting an Exercise Solution

Once the student has completed the exercise, they should commit it to GitHub on a branch, create a PR, and send the link to the instructor.

It is very **important** that the student submit their work on a branch. Otherwise, a PR cannot be created for review by the instructor. It is critical that students learn good version control habits by always committing their work on a branch.

Work can be committed in the VS Code Source Control panel by entering a Commit message and clicking the "Commit" button, followed by the "Sync Changes" button.

Once committed and pushed, the student should switch to GitHub and create a PR. The PR link should then be sent to the instructor using whatever communication technique the instructor has determined (for example, Slack, text message, Google Chat, etc.).

Once the instructor approves the PR, the student should merge it to their `main` branch, and then pull the updated `main` branch to their local VS Code. Ideally, the student would merge a prior exercise before beginning a new one.

Details can be found in the [Submitting Your Solution Guide](./guides/Exercise-Workflow_Submitting-Your-Solution/README.md).

### Q&A Session

Once enough students have submitted their solutions, the instructor will start a Q&A session. The Q&A session usually proceeds with the instructor asking the questions and the students providing the answers! The instructor may provide additional details on the quiz questions, discuss additional concepts relevant to the exercise topic, and demonstrate how to implement the exercise. Students may also be asked to "read" the solution code aloud.
