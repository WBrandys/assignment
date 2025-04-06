# Assignment
Wiktoria Brandys

Date: 06.04.2025

I'm a bioinformatician student on UJ

## Git summary
This is a short guide how to use git.

It contains **the most important commands** and their understanding
### Configuration

```
git config --global user.name "your_username"
git config --global user.email your_email
git config --list
```

### Ssh key
- 

```
ls -al ~/.ssh
ssh-keygen -t ed25519 -C "your_email"
cat ~/.ssh/id_ed25519.pub
ssh -T git@github.com
```
- Last step contains adding SSH key to your GitHub
- It's simple after you copy your SSH key, go to _Settings_,
  then _SSH and GPG keys_ and paste the link

### New repository
1. To create a new repository, you need to click on _New_,
2. Then choose appropriate settings and _Create repository_,
3. Later you need to click _Code_ and copy the SSH link,
4. Last step is to clone a repo:

```
git clone git@github.com:WBrandys/your_repository_name.git 
```

### Adding, committing and pushing

```
git add file_name
git commit -m file_name "commit_info"
git push main origin
```
	- origin is the default name Git gives to the server you cloned from
	- Add `--amend` if you made any mistake in commit message
