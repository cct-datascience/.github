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

If you need any help there are several options:
* create a [new issue](https://github.com/terraref/computing-pipeline/issues/new)
* search the [existing issues](https://github.com/AgPipeline/issues-and-projects/issues) that are open and closed  
* and lastly, email the [maintainer](https://github.com/AgPipeline) of the organization (look for the email address at the top of the page)

Our [OSF site](https://osf.io/tzmhp/wiki/home/) has additional information on [issues and pull requests](https://osf.io/tzmhp/wiki/Issues%20and%20Pull%20Requests/), as well as other information that may be useful.

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

Please refer to our OSF [issues and pull requests](https://osf.io/tzmhp/wiki/Issues%20and%20Pull%20Requests/) page for more information.

## Contributing Text or Code

Please refer to our OSF [issues and pull requests](https://osf.io/tzmhp/wiki/Issues%20and%20Pull%20Requests/) page for more information.

### Overview

When you add a new feature or make other changes, please create an issue first, to allow others to comment and give feedback. 

The preferred workflow for making changes is the [fork](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo) and [branch](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/managing-branches#creating-a-branch) approach.

When you have created a new feature or change to existing code or documentation, create a [Pull Request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests) and solicit feedback.

### Adding Features and Submitting Changes

Always work in a branch rather than directly on the master branch.
Branches should focus on fixing or adding a single feature or set of closely related features making it easier to review and merge your contributions.
If more than one person is working on the same code, make sure to keep your master branch in sync with the master branch of the repository.

Name your branch in a way that makes it easy for others to know what it's for.
For example, include the change(s) to be made, or an issue number, or both.
Examples: `readme_test_instructions`, or `issue_321_blob_support`. 

#### Work and commit

Do you work, and [commit](https://git-scm.com/docs/git-commit) your changes locally as you see fit.
Make your commit messages helpful.

#### Push your changes up to GitHub.

Be sure to [push](https://docs.github.com/en/github/using-git/pushing-commits-to-a-remote-repository) your changes often to save them on the web.
This will allow your changes to be available to other contributors, and yourself as needed.

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
* Let reviewers know of anything they should ignore (for example: "ignore the function behind the curtain") and why

### Reviewing a Pull Request
We recommend reading the following before reviewing Pull Requests: https://github.com/margarethchan/Compassionate-Code-Reviews#compassionate-code-reviews

The goal of a Reviewer is to provide additional feedback on the Pull Request that's not provided by any automation.
For example: it's possible to write complex code that passes syntax checks, styling checks, and testing; if a reviewer knows a simpler way to perform the actions, this might be a good place to suggest changes

## Code Of Conduct

Refer to our [Code Of Conduct](https://github.com/AgPipeline/.github/blob/master/.github/CODE_OF_CONDUCT.md) document.
