## Rite Community

Welcome to Rite Community. 

We’re excited to have you here. This guide will help you get started with our repositories and ensure you’re set up with all the right tools and security practices. 

Please read this note carefully and refer back to it as needed. If you ever feel stuck, don’t hesitate to ask for help — we’re all in this together!

## Setup

Before diving in, please make sure your development environment is ready:

1. `.gitconfig` Setup

To make sure your commits are properly attributed, please set up your `.gitconfig`:

```bash
git config --global user.name "Your Full Name"
git config --global user.email "you@ritecommunity.com"
git config --global init.defaultBranch master
git config --global pull.rebase false
```
For signed commits (required — see below), also set:

```bash
git config --global commit.gpgsign true
```

## Security Policies

We take security and data privacy very seriously. Please make sure the following are in place before contributing:

All commits must be GPG or SSH [signed](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits).
	•	Learn how to generate a [GPG key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh) **or**
	•	Or sign commits with your SSH key (recommended for GitHub).

Add your key to GitHub and verify it’s working, run `git log --show-signature`.

### SSH

You must use SSH to interact with our repositories. Set up SSH as follows:

```bash
ssh-keygen -t ed25519 -C "<username>@ritecommunity.com"
```

Then [add your SSH key](https://github.com/settings/keys) to Github and test it:

```bash
ssh -T git@github.com
```

### Repository Security Guidelines
* Never commit secrets or credentials.
* Always open PRs from feature branches (never commit directly to `master`).
* Review changes for sensitive files or secrets using .gitignore and .gitattributes.
* Enable 2FA on your GitHub account.

### General Contribution Guidelines

Please follow these practices:
* Create a new branch for each feature or bugfixes.
* Write clear, descriptive commit messages.
* Follow the code style outlined in the repo’s `CONTRIBUTING.md` or `.editorconfig` (if one is present).
* Open pull requests early — we believe in collaborative development.
* Add tests when applicable, and always ensure existing ones pass before submitting a PR for approval.
* Be kind and constructive in code reviews.

## Questions or Help?
Please reach out to your respectiev team leads or Andrew for more information. 

 
