# FALL26

Course materials for **DATA 301: Introduction to Machine Learning**.

**This repo is read-only for you.** It is the shared "upstream" that every student
repo syncs from. You don't commit here and you don't open Pull Requests here.
Your actual work happens in your own private repo, `DATA301-F26-<your-username>`.

This is different from DATA 201: there are no team repos this semester. Weekly
assignments are **individual**, and each of you has your own repo.

## Getting the latest content

Run this in *your own* repo whenever new material is announced:

```
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

(First time only: `git remote add upstream https://github.com/MachineLearningUoR/FALL26.git`)

## One-time setup

After you clone your own repo:

```
pip install -r requirements.txt
nbstripout --install
```

`nbstripout` strips notebook outputs from every commit, so `.ipynb` diffs come
from actual code changes instead of from someone re-running a cell. It's in
`requirements.txt`, but you have to activate it once per clone. That part
doesn't happen automatically.

**Read the PyTorch note at the top of `requirements.txt` before you install.**
On Linux the default install is about 2.5 GB of CUDA libraries you don't need.

## Submitting your work

Each weekly assignment follows the same path:

```
git checkout -b hw/week-03
# ...do the work, commit as you go...
git push origin hw/week-03
```

Then open a **Pull Request into `main` in your own repo**. That PR is your
submission. I review it and leave comments inline. Those comments are your
feedback, and merging the PR closes out the assignment.

You're encouraged to add a classmate as a reviewer on your PRs. One rule:
**reviewers comment, reviewers don't commit.** Reading someone else's code and
asking good questions about it is the point; writing it for them is not.

---
*The full workflow (branching, Pull Requests, review, the whole cycle) is on
the last page of the syllabus.*
