# Github pages
## A great way to manage/host static sites for free!

### Let's say your cousin wants you to create a small site for her pet grooming business

* Let's 'fork' a [nice template](http://startbootstrap.com/template-categories/all/) to use. Fork is to create a personal copy of someone else's repository on GitHub.
* We find a [business template](http://startbootstrap.com/template-overviews/modern-business/), click the 'View Source on Github' link and click the 'fork' button on GitHub.
* Select your personal account to fork the repository to if GitHub asks.
* Copy the 'clone url' in the bottom right corner of the page. ![Copy the clone url (bottom right corner of the image)](https://raw.githubusercontent.com/lfucg/code-reviews/master/images/github-repository-location.png)
* In your git client (like git extensions)
  * clone the repository at the url
  * (git extensions) command > branch > create a new branch called 'gh-pages'
  * push the new branch back to github (by clicking push)
* After a couple of minutes, your site will be deployed at the following url: [your-github-username].github.io/[repository-name]. For example: http://eeeschwartz.github.io/startbootstrap-grayscale/
* To customize you site:
  * Make changes on your local machine (on the gh-pages branch), 
  * Check them into git
  * Push them to GitHub, which deploys them in a couple of minutes!





