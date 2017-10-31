# swi1-2017

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


