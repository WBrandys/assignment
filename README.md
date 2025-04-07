# Assignment
Wiktoria Brandys

Date: 06.04.2025

I'm a bioinformatician student on UJ

## Git summary
This is a short guide on how to use Git. 
It contains **the most important commands** and their explanation.
### Configuration
```
git config --global user.name "your_username"
git config --global user.email your_email
git config --list
```

### Ssh key
```
ls -al ~/.ssh
ssh-keygen -t ed25519 -C "your_email"
cat ~/.ssh/id_ed25519.pub
ssh -T git@github.com
```
- Last step contains adding SSH key to your GitHub,
- It's simple, after you copy your SSH key, go to _Settings_,
  then click _SSH and GPG keys_ and paste the link.

### Creating a New repository
1. Go on GitHub and click on _New_,
2. Then choose settings and click _Create repository_,
3. Later you need to click _Code_ and copy the SSH link,
4. Last step is to clone a repository to your machine:

```
git clone git@github.com:user_name/your_repository_name.git 
```

### Adding, committing and pushing

```
git add file_name
git commit -m "commit_info"
git push main origin
```

**Additional tips:**
- "origin" is the default name Git gives to the remote repository,
- Use `commit -m --amend` if you made any mistake in last commit message
- Use `add -u` to 
- To check current changes use `git status`
- To see a difference between commits use `git diff`

### Branching and merging
Branching lets you experiment without affecting the main branch. Later, you can merge changes back.
- Create a new branch:
```
git branch branch_name
```
- Change working branch:
```
git checkout branch_name
```
- Merge another branch into the current one:
```
git merge branch_name
```
Make sure you're on the branch you want to _merge into_ before running the merge.

### More basic commands:
- To see all the commits use:
```
git log
```
- To downloads from remote and merges with local use:
```
git pull
```
- To download changes from remote without merging use:
```
git fetch
```
