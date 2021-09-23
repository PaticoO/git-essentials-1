#LOTS DELETED

## Where to get this course:
- [x] [Git for Everybody.com](https://gitforeverybody.com/git-essentials/)
- [x] [Git Essentials on Skillshare.com](https://skl.sh/2viPzB9)
- [x] [Git Essentials on Udemy.com](https://www.udemy.com/course/git-and-github-tutorial/?referralCode=91132F334DCD0CCAA250)

## Docker (advanced devs only)
If you want a completely new and clean environment to start learning git form scratch, you can use a Docker container. That's what I did for this course. Below are the steps to reproduce the same setup I used in the Git Essentials course:

```bash
git clone git@github.com:KalobTaulien/git-essentials.git
cd git-esentials
docker build -t git .
docker run -itd --hostname "gitforeverybody.com" --name "gitforeverybody.com" git
docker container ls -a
docker exec -it <container_id> bash

# Once inside your Docker container, run these commands:
apt update
apt install vim nano git
export PS1="\[$(tput setaf 6)\]kalob\[$(tput setaf 2)\]@\[$(tput setaf 3)\]gitforeverybody.com: \[$(tput sgr0)\]"
export TERM=xterm-256color

# Now you can run git commands as if you were on a brand new computer. You'll need to generate an SSH key and add it to GitHub.
```

## Contibutors
If you're opening a pull request against this repo, you should put your name (and website, optional) in the list below!

* Kalob Taulien [(website)](https://gitforeverybody.com/)
* _Insert your name and website here_

___

Course created by Kalob Taulien.
