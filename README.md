# Enhacing a Community Library website
A step-by-step procedure to complete the scenario for enhancing the Greenwood Community Library website, simulating the roles of Morgan and Jamie, and practicing collaborative Git workflows.
#
# SETUPS:
### 1. Create and Clone the GitHub Repository
```
got clone https://github.com/Ofrelex/greenwood-library-website.git
```
![git_clone](img/1_gitclone.png)
```
cd greenwood-library-website
code .
```
![cd_to_re](img/2_CD.png)
#
## BASE WEBSITE SETUP (MAIN BRANCH)
### 2. Create Base HTML Files
In VS Code, create the following files:

* home.html

* about_us.html

* events.html

* contact_us.html

Add random placeholder content in each file (e.g., headers, paragraphs).
![html_files](img/3_html_files.png)

### 3. Stage, Commit, and Push to Main
```
git add .
git commit -m "Add base HTML files for main sections"
git push origin main
```
![Stage](img/4_git_add.png)

![Commit](img/5_git_commit.png)

![Push_to_Main](img/6_git_push.png)
#
# MORGAN’S TASK: Add Book Reviews Section
### 1. Create and Switch to a New Branch
```
git checkout -b add-book-reviews
```
![Switch_Branch](img/7_mo_checkout.png)
#
### 2. Add book_reviews.html
Create a new file: book_reviews.html

Add random content:
```
<h1>Book Reviews</h1>
<p>This section contains reviews of popular books from our community.</p>
```
![Add_Contents](img/8_mo_contentadd.png)
#
### 3. Stage, Commit, and Push
```
git add book_reviews.html
git commit -m "Add book reviews section"
git push origin add-book-reviews
```
![Stage](img/9_mo_git_add.png)

![Commit](img/10_mo_git_commit.png)

![Push](img/11_mo_git_push.png)
#
### 4. Create Pull Request on GitHub
Go to GitHub

* Click "Compare & pull request" for add-book-reviews → main

* Add title: “Add Book Reviews Section”

* Click “Create Pull Request”

* Merge the PR once approved.

![Pull_Request](img/12_github_PR.png)

![PR_Title](img/13_PR_Title.png)

![Merge](img/14_merge_PR.png)
#
### 5. Pull Merged Changes Locally
```
git checkout -b update-events
```
![Switch_Branch](img/15_checkout_main.png)

![pull_main](img/16_pull_main.png)
#
### 2. Update events.html
Edit the file with updated info, e.g.:
```
<h1>Upcoming Community Events</h1>
<ul>
  <li>Book Club - June 15</li>
  <li>Storytime for Kids - June 20</li>
  <li>Author Visit - July 5</li>
</ul>
```
![Events_update](img/18_eventsupdates.png)
#
### 3. Stage and Commit Changes
```
git add events.html
git commit -m "Update events page with upcoming community events"
```
![Stage](img/19_git_add.png)

![Coomit](img/20_git_commit.png)
#
### 4. Pull Latest Changes from Main
```
git pull origin main
```
If there's a conflict, resolve it manually in events.html, then:
```
git add events.html
git commit -m "Resolve merge conflict in events page"
```
![pull_main](img/21_git_pullmain.png)

![Stage](img/22_git_add_events.png)

![Commit](img/23_git_commits.png)
#
### 5. Push and Create Pull Request
```
git push origin update-events
```
* On GitHub: Open a Pull Request from update-events → main
* Title: “Update Events Page”
* Create and merge PR

![git_push](img/24_git_push_origin.png)

![GitHub_Events_Update](img/25_github_update_events.png)

![PR](img/26_PR.png)

![PR_Merge](img/27_merge_PR.png)
#
## FINAL STEP: Sync Local Main
```
git checkout main
git pull origin main
```
![Switch_Branch](img/28_checkout_main.png)

![pull_main](img/29_pull_main.png)