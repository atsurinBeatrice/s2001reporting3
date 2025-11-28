# s2001reporting3
2025/11/28 demo
1) Create GitHub repository for a new R project as GitHub user(email based)
- create a non-main branch(e.g. dev branch)
- apply a rule to main branch which prohibits to push to main directly

2) Create a new R project(reporting activity) in mode of version control and using git
- [Important!] Input URL as SSH

3) Update "Global Options" to use GIT and create a SSH key for RStudio user(linux user)
- Create your SSH key
  #e.g. 
  ssh-keygen -t ed25519 -C "atsushi.kitagawa@dxc.com" or RStudio GUI
- Keep secret key on your home and copy public key and register to GitHub(as your SSH key)
- Register GitHub username and email address as follows.
  #e.g.
  git config --global user.email "atsushi.kitagawa@dxc.com"
  git config --global user.name "atsurinange"

4) Enable renv on Environments of "Project Options"

5) Update following R initial settings
- .Renviron     for definition where is global cache
- .Rprofilel    for definition of custom logger to enable logging high-level info

6) Pull your own branch from Remote Repo(GitHub)

7) Create your own Rscripits under the project folder

8) Install required R packages

9) Take a snapshot of renv.lock

10) Commit and push to your own branch.
