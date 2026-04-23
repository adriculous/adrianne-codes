---
layout: ../../layouts/Layout.astro
title: Fixing GitHub Permission Denied Errors When Pushing a Repo
description: Troubleshooting GitHub permission denied errors when pushing a repository and how switching to SSH resolved the issue.
---

# Fixing GitHub Permission Denied Errors When Pushing a Repo

## The Problem

I tried pushing my project and got this error:

![Permission denied error](/images/learn/github-permissions-error.png)

## What I Tried

- Attempted push using HTTPS (even though I normally use SSH)
- Creating a personal access token in GitHub
- Clearing credentials in my Terminal

None of these worked.

## What Actually Worked

Switching from HTTPS to SSH.

Steps:
- Verified SSH key existed in Terminal
- Confirmed existing SSH key was already added to GitHub (no need to generate a new one)
- Changed remote to SSH
- Tested connection with `ssh -T git@github.com`
- Pushed successfully

After switching to SSH, the push finally worked:

![Successful push](/images/learn/github-permissions-success.png)

## Key Takeaways

- GitHub no longer accepts passwords
- SSH is more reliable than HTTPS
- Credential caching can cause confusing errors

## Notes

During my initial commit, I missed the part where the repo showed the HTTPS URL instead of the usual SSH one. I copied the provided terminal commands rather than using the commands I normally use.

I haven’t created repos in a while, so I ended up just following the instructions as provided without thinking too much about it.

It took a few attempts to fix, but I’m glad the solution turned out to be relatively simple.