# swi1-2017

## SWI 1

These are materials for the [Software Engineering 1](http://is.mendelu.cz/katalog/syllabus.pl?kod=PEF:SWI1) course, taught on Mendel University in Brno, autumn 2017.

There's 2 study groups:

   * starting on 2017-09-26 (every 2 weeks, odd weeks), lead by @ZitaNemeckova and @himdel
   * starting on 2017-10-03 (every 2 weeks, even weeks), lead by @romanblanco and @lpichler

---

If you need to contact us, please use the [ManageIQ/welcome](https://gitter.im/ManageIQ/welcome) channel on [Gitter](https://gitter.im). (You'll need a github login anyway.)

---

Student can gain 50 points during lessons.

### 1st lesson:

* visiting Red Hat office including a small tour 
  * meeting at 13:30 in front of the TPB-B building: Purkynova 111 - tram stop "Technologicky park"
* introduction of the course - University of Helsinki’s Software Factory as inspiration, main idea and objectives
* discussion about preferences - writing tests, Selenium, refactoring, debugging, … 

### 2nd (12.5 points) :octocat: :

Introduce Git and GitHub to students. Students should use only console. GUI like SourceTree are forbidden.

Repo: https://github.com/RoadToSoftwareFactory/swi1-2017-odd-git

* git basics - **12.5 pts** *(1pt per used command)*
  * create GitHub account 
  * git clone
  * git remote
  * git pull upstream/origin —ff-only
  * git branch
  * git checkout
  * git diff/status
  * git add
  * git commit
  * git push

---
Student is expected to create one PR to remote repository. **12.5 pts** 

After this lesson student should be able to create a PR to any remote repository (on GitHub) via console.

Any git cheatsheet is allowed. This one is recommended https://github.com/pyvec/cheatsheets/raw/master/basic-git/basic-git-cs.pdf .

*Note: Bring GitHub materials from GitHubEducation swag they send for this class.*

### 3rd (12.5 points) :octocat: :
* recap :point_up:
* git rebase master - solving conflicts **3 pts**
* git rebase -i master (pick, reword, edit, squash/fixup, drop) **5 pts**
* when finished mention one of instructors **2 pts**

All submitted PR should have a feedback comment:

- [ ] git rebase master - solving conflicts **3pts**
- [ ] git rebase -i master (squash) **3pts**
- [ ] git rebase -i master (reword) **2pts**
- [ ] git rebase -i master (drop) **1pts**
- [ ] git rebase -i master (edit) **2pts**
- [ ] one of instructor mentioned **1.5pts**


---
Student is expected to follow instructions and create one PR to remote repository. 

*Note: First student to complete all tasks successfully will be given GitHub t-shirt gift card. Stickers for everyone.* 

### 4th:

Introduction of ManageIQ. How it works. Architecture. Specs. @miq-bot. Travis. Code climate. Clone repos. 

### 5th (12.5 points):

Static analysis of code. Introduction of following tools for Ruby:

##### FLOG

- code pains
- score - lower is better

https://github.com/seattlerb/flog

Install: `gem install flog`

Run: `flog [file/s]`

##### REEK

- code smells

https://github.com/troessner/reek

Install: `gem install reek`

Run: `reek [options] [file/s]`

##### FLAY

- code similarities

https://github.com/seattlerb/flay

Install: `gem install flay`

Run: `flay -u —diff [file/s]`

##### DEBRIDE

- unused methods

https://github.com/seattlerb/debride

Install: `gem install debride`

Run: `debride [options] [files]`

Alternative: https://github.com/danbernier/zombie_scout

---

Student will be given results from `debride` and will classify them to `false/true`. Each `false` should have a reason (method is called dynamically, `before/after_action`, method is called, aliases,…). **12.5 pts**

### 6th (12.5 points):
Student will verify a report from previous lesson done by his/her classmate. **6.25 pts**

Student will try to lower score given by FLOG for one method. **6.25 pts**

### 7th:
Removal of unused methods - first PR (extra points?). Anything not covered in previous lessons.

--- 


## SWI 2

These are materials for the [Software Engineering 2](https://is.mendelu.cz/katalog/syllabus.pl?predmet=108590;lang=cz) course, taught on Mendel University in Brno, spring 2018.

There's 2 study groups:

   * Tuesday - Javascript, lead by @ZitaNemeckova and @himdel
   * Thursday - Ruby, lead by @romanblanco and @lpichler

---

If you need to contact us, please use the [ManageIQ/welcome](https://gitter.im/ManageIQ/welcome) channel on [Gitter](https://gitter.im). (You'll need a Github login anyway.)

---
This semester will be more focused on individual work. Each group will be given work to do but you can ask for work that is more interesting for you. There is no strict schedule or one-time graded lessons. Attendance is strongly advised.


## Basic info

Never use master branch! `git branch` will show you all your branches and one with * is active branch.

`git checkout -b <name>` creates new branch and switches to it

`git checkout <name>` change active branch

`git status` shows which files where changes/deleted/created

`git diff` shows changes

`git add <file>` adds file to a commit

`git commit` commits changes

`git push origin <branch name>` pushes commit(s) to your repository and it's added to your PR or you can create one

`bin/update` updates 

`bundle exec rails s` runs server. Must be run from manageiq not manageiq-ui-classic

`rake environment jasmine` runs Jasmine tests on localhost:8888

Feel free to suggest anything that should be here.

---


### Tuesday group (Javascript)

Main focus will be on refactoring. We will refactor old controllers to Angular.js component. Then we will rewrite it to React component. Each student will have one controller to work on.

Here are some interesting blogposts/guides/tutorials. It's highly individual which ones will be useful to you so feel free to skip anything. If you read anything that should make this list feel free to contribute.

[Javascript Basic Intro](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Introduction) is quick introduction to fundamental concepts of js. It's a quick read for someone who has some programing experience. You can continue [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript) if you need more materials to study.

[Javascript Intro with more details](https://developer.mozilla.org/cs/docs/Web/JavaScript/A_re-introduction_to_JavaScript) is a bit longer introduction that explains mainly types in js.

[Angularjs Documentation](https://docs.angularjs.org/guide) is the best place to look for anything Angularjs related. You don't have to read whole documentation :)

[Components in Angular.js](https://docs.angularjs.org/guide/component) is detailed description of components and its principles. 

[Blogpost about quality components](https://www.sitepoint.com/building-angular-1-5-components/) is good if you want to read a bit on good practise.

[Refactoring controllers to components in Angular.js](https://teropa.info/blog/2015/10/18/refactoring-angular-apps-to-components.html) is a blogpost that we used as an inspiration for refactoring old Angular.js controllers. We went from controllers to controllers as vm so far. Keep in mind that we are not gonna go as far as Angular 2/4. But you can try it if you really want to but it won't get merged. 

[When you feel tired of it all](https://teropa.info/blog/2015/07/15/overcoming-javascript-framework-fatigue.html) is nice inspirational blogpost when you feel tired of learning new stuff. It's focused on Javascript frameworks but the main ideas about learning go far beyond. You should read it when you need to overcome lack of motivation to learn something new. 

[Make Google your friend](https://www.youtube.com/watch?v=ftQ6A3DKKeg) and the Cloud is the limit :) No kidding, knowing how to find stuff is a must for a good programmer and it's not that hard ;)


#### Convert controller as to component

You can see basic steps in [example PR](https://github.com/ManageIQ/manageiq-ui-classic/pull/2166). This PR was never merged because it was Proof of Concept.

---

### Thursday group (Ruby)
