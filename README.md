# Gym_Git_Exercise_Solutions

## Bundle 1 

### Exercise 1
```bash
git config --global init.defualtBranch master
touch one.html
git branch -m master main
git push -u origin main
git add .
git commit -m "Added an html file"
git remote add origin https://github.com/GunnerBel/Exercise_Git.git
git push -u origin main --force
git checkout -b dev
git checkout -b test
git checkout  dev
git branch -D test
```

### Exercise 2
``` bash
touch home.html
git stash save 'home.html changes'
touch team.html
git stash save 'team.html changes'
touch about.html
git stash save 'about.html changes'
git stash pop
git stash list
git stash pop stash@{1}
git add .
git commit -m "Added home and about pages"
git push origin main
git stash list
git stash pop stash@{0}
git reset --hard 0fd0e013380fe4fef609a6279549ccac53bf6d50
```

## Bundle 2
### Exercise 1

``` bash
git branch ft/bundle-2
git checkout ft/bundle-2
git add services.html 
git commit -m "Added new services page"
git push origin ft/bundle-2
```
### Exercise 2

``` bash
git checkout main
git pull origin main
git checkout -b ft/service-redesign
git add service.html
git commit -m "added a new paragraph to service.html page"
git push origin ft/service-redesign
git checkout main
git add service.html
git commit -m "Added new paragraph to service.html page"
git push origin main
git checkout ft/service-redesign
git checkout ft/service-redesign
git merge main
git add service.html
git commit -m "merged main with service redesign"
git push origin ft/service-redesign

```

### Bundle 3
##  Exercise 1

``` bash
git checkout -b ft/team-page
vi team.html
git add team.html
git commit -m "Added new team page"
git push origin ft/team-page
git checkout main
git checkout -b ft/contact-page
git checkout ft/team-page
git log
git checkout ft/contact-page
git cherry-pick 
touch contact.html
git add contact.html
git commit -m "Added new contact page"
git push origin ft/contact-page
git checkout -b ft/faq-page
touch faq.html
git add faq.html
git commit -m "Added new faq page"
git push origin ft/faq-page
git checkout ft/team-page
git revert 5b3c33ee1343a8b19f9de28482f28a13eaf95bb1
git push origin ft/team-page
```

## Exercise 2
``` bash
git checkout -b ft/home-page-redesign ft/faq-page
git checkout main
touch README.md
git add README.md
git commit -m "Updated README.md"
git push origin main
git checkout ft/home-page-redesign
git rebase main
vi home.html
git add index.html
git commit -m "Added new home page"
git push origin ft/home-page-redesign
```

###  Bundle 4
## Exercise 1

``` bash
git checkout main
git remote add git-copy https://github.com/GunnerBel/New-Exercise.git
git add index.html
git commit -m "Updated home page"
git push origin main
git push git-copy main
```
## Exercise 2

``` bash
git checkout -b ft/footer
git add index.html
git commit -m "Added footer section"
git add index.html
git commit -m "Added contact link to footer"
git push origin ft/footer
git checkout main
git checkout -b ft/squashing
git merge --squash ft/footer
git commit -m "Footer changes squashing"
git push origin ft/squashing
```

### Bundle 5
## Exercise 2
``` bash
git clone https://github.com/GunnerBel/git-cafe-exercise.git
git add index.html
git commit -m "Updated index.html"
git push origin main
```

### Bundle 6
## Exercise 1

```bash
git checkout main
git checkout -b ft/menu
git add menu.html
git commit -m "Added new menu page"
git push origin ft/menu
```

## Exercise 2

``` bash
git checkout main
git checkout -b bugfix/title-change
git add index-4.html
git commit -m "Changed title of index-4.html"
git push origin bugfix/title-change
```

## Exercise 3
``` bash
git add index-4.html
git commit -m "Changed telephone number on contact page"
git push origin hotfix/telephone-change
```

