# BSA Git & GitHub Workshop

Practice Git with your own fork, then create a GitHub profile README.

## 1. Fork and clone

Click **Fork** at the top of this repository and create a fork in your account. Clone your fork (replace YOUR-USERNAME with your GitHub username):

```bash
git clone https://github.com/YOUR-USERNAME/bsa-git-workshop.git
cd bsa-git-workshop
git status
git switch -c practice-readme
```

## 2. Edit and commit

Open `profile-template.md` in an editor. Personalize a few lines and save it.

```bash
git status
git diff
git add profile-template.md
git commit -m "Personalize profile template"
git push -u origin practice-readme
```

On GitHub, open a pull request **within your fork** from `practice-readme` into your fork's `main`. Ask a partner to review it, then merge it. You do not need write access to the original repository.

## 3. Make it your profile README

Create a **public** repository named exactly your GitHub username and initialize it with a README. If it already exists, use it instead. Clone it and edit its root `README.md`; copy ideas from the template if you like.

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-USERNAME.git
cd YOUR-USERNAME
git switch -c update-profile
# Edit README.md and save it
git status
git diff
git add README.md
git commit -m "Update profile README"
git push -u origin update-profile
```

Open a pull request in your profile repository and merge it into the default branch. Visit your GitHub profile to see your README. The template in the workshop repository will not appear there by itself.

## Troubleshooting

- Run `git status` whenever you are unsure what is staged or which branch you are on.
- If Git asks for your identity, set `git config --global user.name "Your Name"` and `git config --global user.email "your-email@example.com"`. GitHub's noreply email is an option.
- If prompted while pushing, follow your Git client's GitHub authentication flow. Account passwords do not work for HTTPS Git operations.
- Share only what you want public. Never commit passwords, tokens, or private data.
