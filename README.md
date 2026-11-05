# 👋 M1A0: Hello World

[![Made with Codex](https://img.shields.io/badge/Made_with-Codex-D97757?logo=anthropic&logoColor=white)](https://tjakoen.github.io/notes/ten-times-zero)
![Dart](https://img.shields.io/badge/Language-Dart-0175C2?logo=dart&logoColor=white)

Your first ADET activity is small on purpose: run a Dart program, save it in GitHub, and submit the exact version you finished. By the end, you should know that your tools and your submission path work.

## 1. Create your private activity repo

Accept your invitation to [HAU-6ADET](https://github.com/HAU-6ADET) first. Sign in with your own GitHub account, then use this public starter to create your private activity repository:

1. Choose **Use this template → Create a new repository**.
2. Set **Owner to HAU-6ADET**. The repository belongs in the course organization unless the instructor explicitly specifies otherwise.
3. Name it with your class's prefix below, followed by your GitHub username. Copy only the row for your class.
4. Choose **Private**. Keep your personal details in that private copy, never in this public template.

| Class | Required prefix | Example only, using a fictional username |
| --- | --- | --- |
| NW-301, Wednesday | m1a0-2223- | m1a0-2223-yourusername |
| WD-302, Thursday | m1a0-2293- | m1a0-2293-yourusername |
| EMC-202, Friday | m1a0-2182- | m1a0-2182-yourusername |
| WD-303, Friday | m1a0-2294- | m1a0-2294-yourusername |

Replace “yourusername” with your actual GitHub username. Do not use the template's classcode/yourname placeholders. The Friday classes retain separate class codes even when taught together; use the code shown in your own Canvas course.

If HAU-6ADET is missing from the Owner list, ask the instructor to check your invitation. Do not create a personal-account replacement. If the instructor already assigned you an activity repository, use that one instead of creating a duplicate.

## 2. Clone and open your activity repo

Open your new private repository, choose **Code → HTTPS**, and copy its clone URL. In your terminal, run git clone followed by the copied URL. Then run cd followed by the name of the newly created folder. Open that folder in your editor, and run all commands below from inside it.

Verify where your pushes will go:

```sh
git remote -v
```

The remote must point to HAU-6ADET and your own M1A0 repository. This activity repo is separate from your student workspace, which holds notes and planning. Do not clone the teacher repository or write this program in the workspace instead.

You need Git and Dart 3.12 or later for local work. Follow the class setup instructions if either is missing. If your instructor enables Codespaces, this template includes a Dart development-container configuration. Local Dart checks have been verified; the Codespaces launch itself still needs a class setup check.

## 3. Complete Hello World

Install the activity's dependencies:

```sh
dart pub get
```

Open bin/hello.dart. Inside main(), write a statement that prints exactly this greeting on one line:

```text
Hello, World!
```

The comma, capital letters and exclamation mark matter. Run the program:

```sh
dart run bin/hello.dart
```

In your private copy, fill in student.json with your name, student number, school email, class code and GitHub username. Use the same verified identity for the course. Keep all values as text, including the student number and class code.

## 4. Check and save your work

```sh
dart analyze
dart test
```

The checks cover the greeting and your required identity fields. They fail on the untouched starter because both are intentionally blank. Fix your program and details; do not edit the tests to make them pass. A green student-side check is useful feedback; the instructor grades from trusted course checks.

Review your changes before committing. Only the activity files belong here; never commit credentials or unrelated personal files.

```sh
git status
git add bin/hello.dart student.json README.md pubspec.lock
git commit -m "Complete M1A0 Hello World"
git push
```

If GitHub asks you to authenticate, use your configured GitHub sign-in method. Never put a token in a source file, README, screenshot, or submission comment.

## 5. Submit the exact commit link in Canvas

A push saves your work. You still need to submit it:

1. Open your private M1A0 repository on GitHub.
2. Open its commit history and select the commit containing your finished work.
3. Copy that commit page's full URL. It contains **/commit/** followed by the full commit identifier.
4. Open **M1A0 in your own Canvas course** and submit that link using the Website URL option.
5. Reopen the Canvas assignment and verify that your submitted link points to the intended commit.

Submit the commit page, rather than the repository home page, a branch link, or a screenshot. The instructor needs access to the repository. Your repository stays private; report an access problem instead of making it public. If you revise your work, submit the new commit link through Canvas while the assignment allows resubmission. A later push does not change the commit you already submitted.

The Canvas assignment, deadline and points will be announced in your class. This public template does not create a Canvas assignment or set a score. The current week-one route is a direct Canvas URL submission; you do not need to submit again through Course Platform.

## AI and other assistance

Follow the rules in the activity brief and the instructor's AI policy. Use permitted help to understand setup, syntax and errors, then test and explain your own submission. Disclose the tool and how it helped in the section below. Ask the instructor first if permission is unclear. Never share credentials, personal information or another student's private work with a tool.

In your private copy, replace this sentence with “No AI assistance used” or a short description of the tool, what it helped with, and what you kept or changed. Credit any other code or references you reuse.

## If something fails

Tell the instructor which step failed, what the error says, and what you tried. Share private links through the course's approved channel. Do not post your student details or credentials in this public repository's issues.

---
🤖 **Built with Codex. I don't prompt and pray, I prompt and prove.** Every commit here is co-authored with an AI, on purpose. [How I actually work with AI, receipts and all →](https://tjakoen.github.io/notes/ten-times-zero)
