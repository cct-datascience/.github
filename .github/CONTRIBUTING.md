# How to contribute

Your contributions are highly encouraged. 
Our goal is to keep it as easy as possible for you contribute changes that get things working in your environment. 
There are a few guidelines that we need contributors to follow so that we can have a chance of keeping on top of things.

There are many ways to get in touch:

* report bugs
* request features
  * support for existing databases / APIs
  * integrating existing algorithms into the pipeline
* join discussion of open issues, features, and bugs at AgPipeline/issues-and-projects/issues
* contribute algorithms to the pipeline
* revise documentation

New features are directed toward developing and extending the AgPipeline computational infrastructure. 

If you need any help, please create a [new issue](https://github.com/terraref/computing-pipeline/issues/new).

## Related Projects

This pipeline combines a number of related projects. 
In many cases, new features may be discussed in this repository but eventually added directly to existing software. 
In these cases, please link the issues across repositories (e.g. add `will be implemented by pecanproject/bety#123` to the issue.

Some of the related software we will be using and contributing to.

* BETYdb: github.com/pecanproject/bety
* Breeding Management Systems
* PlantCV (image processing): https://github.com/danforthcenter/plantcv

## Creating Issues

- Make sure you have a GitHub account.
- Search GitHub and Google to see if your issue has already been reported
    - Create an issue in GitHub, assuming one does not already exist.
	- Clearly describe the issue including steps to reproduce when it is a bug.
	- Make sure you fill in the earliest version that you know has the issue.
- Ask @dlebauer or @chris-schnaufer to add you to the AgPipeline project if you plan on fixing the issue.

## Contributing Text or Code

### Overview

When you add a significant **new feature**, please create an issue first, to allow others to comment and give feedback. 

When you have created a new feature or non-trivial change to existing code, create a [Pull Request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

**Branching and Pull Requests**: Although many core developers have write permissions on the AgPipeline repositories, 
_please use the feature branch workflow_ (below) in order to allow pull requests, automated testing, and code review.


### Web and Desktop Interfaces

If you haven't used git before, the GitHub website and GitHub desktop client allow you to do all of the following within a graphical user interface. The GitHub interface is often the easiest way to make changes even if you do know git. These make contributing easy and fun, and are well documented.

Any file can be edited in the GitHub interface, and new files can be created. 
GitHub will create these as a new pull request.

### Using Git at the Command Line for GitHub

Configure your local instance of [git](https://git-scm.com/doc).
Make sure you use an email associated with your GitHub account.

```bash
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

[Fork this repository](https://github.com/AgPipeline/issues-and-projects.git)

Clone your fork of this repository

```bash
git clone https://github.com/<your username>/issues-and-projects.git
```

Setup repository to be able to fetch from the master

```bash
git remote add upstream https://github.com/AgPipeline/issues-and-projects.git
```

### Adding Features and Submitting Changes

Always work in a branch rather than directly on the master branch.
Branches should focus on fixing or adding a single feature or set of closely related features making it easier to review and merge your contributions.
If more than one person is working on the same code, make sure to keep your master branch in sync with the master branch of the repository.

Here is a simplified workflow on how add a new feature:

#### Update to the latest version

Update your master (both locally and on GitHub)

```bash
git fetch upstream
git checkout master
git merge upstream/master
git push
```

#### Create a branch to do your work.

A good practice is to call the branch in the form of GH-<issue-number> followed by the title of the issue. This makes it easier to find out the issue you are trying to solve and helps us to understand what is done in the branch. Calling a branch my-work is confusing. Names of branch can not have a space, and should be replaced with a hyphen.

```bash
git checkout -b GH-issuenumber-title-of-issue
```

#### Work and commit

Do you work, and commit as you see fit. Make your commit messages helpful. 

#### Push your changes up to GitHub.

If this is the first time pushing to GitHub you will need to use the extended command, otherwise you can simply use `git push`.

```bash
git push -u origin GH-issuenumber-title-of-issue
```

### Pull Request

When finished, create a Pull Request from your branch to the main repository.
Keep in mind that when making a Pull Request, the idea is to provide enough relevant information so that reviewers know what is expected of them, and can understand the changes made.

We recommend reading the following before making a Pull Request: https://github.blog/2015-01-21-how-to-write-the-perfect-pull-request/

There is a Pull Request template that needs to be filled out when making a Pull Request and most of the information needed should be self-explanatory.

Be sure to **leave notes for different reviewers** as to what their expected role would be.
For example, let non-technical people know that you want them to test out a feature and not critique the code; be sure to provide information on where it can be tested out.
Use the `@mention` functionality in GitHub when providing this information.

Some things to keep in mind:
* if there are automated CI (Continuous Integration) checks performed, there's no need for reviewers to perform those tasks
* If the CI performs style reviews (such as using `pylint`) reviewers don't need to do that
* If the CI performs testing reviewers again don't need to do that. However, reviewing test scripts and such can be part of the review
* Let reviewers know of anything they should ignore (for example: "ignore the man behind the curtain") and why

### Reviewing a Pull Request
We recommend reading the following before reviewing Pull Requests: https://github.com/margarethchan/Compassionate-Code-Reviews#compassionate-code-reviews

The goal of a Reviewer is to provide additional feedback on the Pull Request that's not provided by any automation.
For example: it's possible to write complex code that passes syntax checks, styling checks, and testing; if a reviewer knows a simpler way to perform the actions, this might be a good place to suggest changes

## Code Of Conduct

Refer to our [Code Of Conduct](https://github.com/AgPipeline/.github/blob/master/.github/CODE_OF_CONDUCT.md) document.
