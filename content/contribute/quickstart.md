+++
author = "Hugo Authors"
title = "Quickstart guide"
date = "2024-03-18"
description = "A quickstart guide to creating your Solution Pattern’s Website"
tags = [
    "markdown",
    "text",
]
headerimage = "images/contribute/quickstart.png"
cssclass = "col-12 col-md-6 col-lg-3"
externalurl = "https://redhat-solution-patterns.github.io/solution-patterns/contributors-quickstart.html"
+++


Run through this 15-minute ![](image::/images/apim/image::/images/imagesection[].png) to get started quickly. 

<!--more-->

## Prerequisites

Before getting started, make sure to have the following CLI tools installed on your local machine: 
* git
* node
* npm (>=12.13.0) and 
* gulp

## 1. Creating a new project 

To save you some time and quickly get started documenting, we'll use as a foundation the [Solution Pattern website template](https://github.com/redhat-solution-patterns/solution-pattern-website-template). 

* Open the https://github.com/redhat-solution-patterns/solution-pattern-website-template[template's repository] and click on the green button *"Use this template"* and choose *Create a new repository*; 

![Scenario 1: Across columns](/create-repo-button.png)



* Choose the following options in *Create a new repository* page that is displayed:
* Check the *Include all branches* to ensure the github pages are deployed correctly.
* Enter your repository name (e.g. `solution-pattern-xyz`) and a description
* Choose an appropriate *Owner* (your personal account or one of your organizations). Once you're ready to publish your first version, you can move or fork the repository into the https://github.com/redhat-solution-patterns[redhat-solution-patterns] organization. 
* To avail of github pages to publish your documentation, keep the repository as *Public*.
* Click on *"Create repository"*;

![Scenario 1: Across columns](create-new-repo-page.png)

* In a few seconds your repo will ready for use. 

## 2. Building and Running the project

Next, let's build and run the project on development mode. 

* Clone the *new* repository to your local machine using `git clone` from your local CLI.

> You can rely on hot-reload features during your development; therefore, you'll save time validating your implementation's output results.


* In a terminal, navigate to your project's repository;
* Build and start the project with:

```html
npm install
npx gulp
```


* A new page should open on your browser pointing to [http://localhost:3000/solution-pattern-template/index.html](http://localhost:3000/solution-pattern-template/index.html)


## 3. Next actions

* Get familiar with  [the project's structure]({{< relref path="indepth-guide.md" >}}).
* Know the available capabilities xref::contributor-in-depth.adoc#_language_and_components[to complete your document].
* Learn how to xref::contributor-in-depth.adoc#_4_publish[publish the pattern] as a github page.
