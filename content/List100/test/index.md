---
title: Basic Git Commands
subtitle: Some useful commands for git
summary: This post contains all the basic initial commands for initializing or publishing a repo
# description:
# slug: basic-git-commands
# authors:
#     - Ukant Jadia

draft: false
date: 2023-12-30T14:15:59+05:30
lastmod:


featured: true
projects: []

image:
    # caption: 'Image credit: Ukant'
    focal_point: ''
    placement: 1
    preview_only: false

categories:
    - Version Control System-VCS
tags:
    - Git
    - Basics
    - Linux
---


# what you should do in git
1. git init -b main
2. git remote add origin <repo_link>
3. git remote -v



## List 100

> Things I want to do before I die. Please let me know if you have any recommendation.
> Progress as of Dec 31, 2023: 40.75/92.
> Things I want to do before I die. Please let me know if you have any recommendation.
> ✅ Learn Spanish
> ✅ Live in another country


**✔**


---

(:smile) sdfsafd
✓ Start a nonprofit organization
✗ See my book being sold at an airport outside Vietnam
✓ Be in a movie/commercial (I’ve actually done this in 3 countries: Vietnam, India, US)
✗ Become the first author of a paper at a top-tier conference
✗ Get published on the New Yorker
---

- ✗ Read 1000 books (~60% done)
- ✓ Teach a graduate-level course
- ✓ Start a company
- ✗ Author a patent

---
✗ Write for a TV show that I watch
----
```bash
cd to the root file of the project
echo "+ Project " >> README.md
git init
git add .
git commit -m "README"
git branch -M Main
git remote add origin <repo_link>
git push -u origin Main
```
----
+ pushing an existing repo from cli
git remote add origin https://github.com/UserCtf777/Inkdrop.git
git branch -M Main
git push -u origin Main



---
after clonning any repo it have the address of origin, simply you cannot add your repo url for backup/project/ICR
for that you have to change the origin url follow the following command

+ to check the origin url try the remote verbose
git remote -v

+ to change the remote origin try
git remote set-url origin <repo_url>



---
+ new error found
+ sometimes when we clone the repo we use depth=1 to remove it's history
+ this give the error during pushing it to other origin
+ error looks like
+          ![remote rejected] Main -> Main (shallow update not allowed)
+	    error: failed to push some refs to

+ to solve this try
git remote set-url <old_url>
git fetch --unshallow old
1. git init -b main
2. git remote add origin <repo_link>
3. git remote -v


----

cd to the root file of the project
echo "+ Project " >> README.md
git init
git add .
git commit -m "README"
git branch -M Main
git remote add origin <repo_link>
git push -u origin Main

----
+ pushing an existing repo from cli
git remote add origin https://github.com/UserCtf777/Inkdrop.git
git branch -M Main
git push -u origin Main



---
after clonning any repo it have the address of origin, simply you cannot add your repo url for backup/project/ICR
for that you have to change the origin url follow the following command

+ to check the origin url try the remote verbose
git remote -v

+ to change the remote origin try
git remote set-url origin <repo_url>



---
+ new error found
+ sometimes when we clone the repo we use depth=1 to remove it's history
+ this give the error during pushing it to other origin
+ error looks like
+          ![remote rejected] Main -> Main (shallow update not allowed)
+	    error: failed to push some refs to

+ to solve this try
git remote set-url <old_url>
git fetch --unshallow old
+!/bin/bash

cd ~/work/obs/Obsidian

git add .
git commit -m 'daily update'
git push

+!/bin/bash

+ to make dir work as git repo
git init

+ to check the changes
git status

+ to sort/simplify the changes
git add .

+ git log shows the log of all commit done
git log

+ restore to discard the changes
git restore .

+ to commit the changes [with '-m' for successful commit/{-m => metadata of changes}]
git commit -m "daily update"

+ git push to add new file to the repo
git push



+ command to add remote repo / it skip the authentication part during git push
git remote add origin git@github.com:UserCtf777/Obsidian.git
git branch -M master
git push -m origin master

+ To solve the conflicts during rebasing
git rebase --continue + fix conflicts and run this
git rebase --skip + to skip this patch/changes
git rebase --abort + to checkout the original branch

+ When we have unresolved conflicts before merging or having error related to add
git fetch + to gain the latest changes from server
git merge origin master + to give a try to automatice merging
+ it will only work if branch has to merge something-- it can be checked with git status
git merge --abort  + the unresolved conflicts will be cleared off

+ to edit the conflicts
git rebase --edit-todo
git rebase --continue

+ if conflicts dosen't resolve then
git rebase --abort
+ it will give the path of unresolved files
+ if you know how to edit then resolve them
+ OR you can remove that confict by
git rm <file>
+ if nothing is ahppening you can skip the commit wiht
git rebase --skip


"List 100
Things I want to do before I die. Please let me know if you have any recommendation.
Progress as of Dec 31, 2023: 40.75/92.

✓ Learn Spanish
✓ Live in another country
✓ Start a nonprofit organization
✗ See my book being sold at an airport outside Vietnam
✓ Be in a movie/commercial (I’ve actually done this in 3 countries: Vietnam, India, US)
✗ Become the first author of a paper at a top-tier conference
✗ Get published on the New Yorker
✗ Read 1000 books (~60% done)
✓ Teach a graduate-level course
✓ Start a company
✗ Author a patent
✗ Write for a TV show that I watch
✗ Design and publish a game
✓ Fall in love
✓ Build a home (a simple one, but it’s mine)
✗ Have a salad from my garden
✗ Become a parent
✗ Be a writer in Paris
✓ Go on a trip overseas with my whole family
✗ Take a hot-air balloon ride
✓ Be in a submarine
✗ Swim a mile
✗ Run a half marathon
✗ Scuba dive
✓ Learn to ski
✓ Surf in Hawaii
✓ Fly an airplane
✓ Learn to drive a car
✗ Get a PhD (in CS, Neuroscience, or Psychology)
✗ Body transformation
✓ Dance on stage at a concert (thanks Flo Rida!)
✗ Ride a horse in Mongolia
✓ Publish a Python package
✗ Create my own programming language
✗ Start a scholarship to support brave young kids
✗ Volunteer 1000 hours to help to the elderlies
✗ Get involved in a publishing house that focuses on math, science, and engineering books
✗ Start a research lab
✓ Take a walk in the rain
✓ Eat at a 3 Michelin star restaurant
✓ Ask a stranger out (he said no)
✓ Invite a stranger to my home (CouchSurfing)
✗ Sleep in a castle
✓ Sleep outside on the beach, under the sky (Eilat, Israel)
✓ Go on an African safari
✓ Camp in a desert
✗ See auroras
✓ Learn to salsa
✗ Learn to play a music instrument (tried 3x)
✗ Zero gravity
✓ Work in a casino
✓ Do stand-up
✓ Travel Southeast Asia
✓ Hitchhike across Africa (Egypt to Mozambique)
✗ Spend at least a month in Western Africa
✓ Hike Los Andes
✓ Visit South Omo valley, Ethiopia
✗ Sail around the Caribbean
✗ Drink vodka in Russia
✗ Eat sushi in Japan
✗ Travel around Eastern Europe
✓ See Kashmir
✗ Visit Mecca
✓ Do the Bible tour: Jerusalem, lake of Galilee, Jordan river, Bethlehem, Nazareth
✗ Stay with an Amazonian tribe
✓ Visit an Amish community
✗ Visit Vatican
✗ Visit Tehran
✗ Visit Sicily
✗ Visit 100 countries (~40% done)
✗ Go to South Pole or North Pole
✓ Climb Great Pyramid of Giza, Egypt
✗ Climb Great wall, China
✗ Hike to Everest base camp
✗ Reed Dance, Swaziland
✗ Burning Man, the US
✗ Carnival in Brazil
✓ Watch a Broadway show in New York
✓ Pashut Festival, Israel
✓ Laos’ new year
✗ Watch bullfight in Spain
✗ Watch a soccer game at Camp Nou (Old Trafford is fine too)
✓ Visit Googleplex
✗ Speak at TED
✗ Meet the Pope
✗ Meet a prince
✗ Meet JK Rowling
✓ See a comet
✓ Meet Dalai Lama
✗ Have my own ice cream flavor
~ Be awesome
~ Be kind
P.S.: I spend a lot of time thinking about how to live, and occasionally write about it."
