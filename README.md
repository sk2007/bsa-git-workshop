# BSA Git & GitHub Workshop

First, build a GitHub profile README. Then practice branches and pull requests in a fork of this workshop repository.

## Exercise 1: Your profile README

1. On GitHub, create a **public** repository named exactly your GitHub username. Turn on **Add README**. If it already exists, use it instead.
2. On your repository, click **Code → HTTPS** and copy the URL. Open a terminal and run:

```bash
git clone YOUR-COPIED-URL
cd YOUR-USERNAME
git status
```

Replace the placeholders with your copied URL and username. Open the folder in your editor, edit its root `README.md`, and save. You can use ideas from [profile-template.md](profile-template.md).

```bash
git status
git diff
git add README.md
git status
git commit -m "Update profile README"
git push
```

Complete GitHub sign-in if prompted. Refresh the repository, then visit your GitHub profile. Your README appears when the repository is public, named after your username, and has a root README.md on its default branch.

## Exercise 2: Fork and open a pull request

Click **Fork** at the top of this repository to create your own copy. Clone your fork; replace YOUR-USERNAME below.

```bash
git clone https://github.com/YOUR-USERNAME/bsa-git-workshop.git
cd bsa-git-workshop
git switch -c practice-readme
```

Edit and save `profile-template.md`, then:

```bash
git status
git diff
git add profile-template.md
git commit -m "Personalize profile template"
git push -u origin practice-readme
```

Open a pull request **within your fork** from `practice-readme` into your fork's `main`. Check the base repository: GitHub may suggest the original repository. Ask a partner to review, then merge.

## Troubleshooting

- Run `git status` whenever you are unsure what is staged or which branch you are on.
- If Git asks for your identity, set `git config --global user.name "Your Name"` and `git config --global user.email "your-email@example.com"`. GitHub's noreply email is an option.
- If prompted while pushing, follow your Git client's GitHub authentication flow. Account passwords do not work for HTTPS Git operations.
- Share only what you want public. Never commit passwords, tokens, or private data.
