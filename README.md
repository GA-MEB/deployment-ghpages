[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Deploying to GitHub Pages

<!--
  title: Deploying to GitHub Pages
  type: lesson
  estimated duration: 30 min
  creator: Matt Brendzel
  competencies: git, GitHub, deployment
-->

## Objectives

  At the end of this session, you should
  (with the help of a reference, and a little time)
  be able to:

  -  Deploy a static site to GitHub Pages.

## Prerequisites

You should already be able to:

  -  Create a new Git repository.
  -  Add and commit changes.
  -  Build a static HTML page.
  -  Create and use Git branches.

### Read: Deploy a Site to GitHub Pages

You've learned how to make a web page, and publish it to GitHub, but you haven't
yet learned about how to **deploy** your page so that it's accessible from the
world wide web.

GitHub provides a hosting service called GitHub Pages which allows you to push
up a site to GitHub as a repository, and have it be automatically deployed on
GitHub's servers at a unique URL.

Take a quick read through the [official website](https://pages.github.com/)
to get a sense for how the process works.

### Code Along: Deploy a Site to GitHub Pages

Deploying a site on GitHub Pages is actually quite straightforward.
Your repository simply needs to have a branch called `gh-pages`, and on that
branch, the HTML needs to be in a file in the root of the repo called
`index.html`. That's it!

Let's walk through how that might work in the context of a larger project.

1.  Create a new directory called `example-site`, and turn it into a Git repo.

2.  On the `master` branch, let's create a file called `index.html` and fill it
    with boilerplate HTML.

3.  Next, let's add some HTML content and make a commit.

4.  Create a new branch (`gh-pages`) at the end of the master branch.

    Now, both of GitHub Pages's requirements are met.

5.  Make a new empty repository called `example-site` on GitHub, and set it as
    the `origin` remote repo. Push up the `gh-pages` branch.

6.  The URL for our new deployed page will be
    `<yourGitHubUsername>.github.io/<repositoryName>`.
    Check it out in the browser!

>   If for whatever reason `index.html` is not in the root of the repo, the URL
>   for the page will be
>   `<yourGitHubUsername>.github.io/<repositoryName>/<pathToIndex.html>`
