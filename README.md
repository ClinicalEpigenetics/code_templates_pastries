# code_templates

A Repo for common and re-useable worflows. Intended for lab members to clone or fork into their projects to speed things up.

## Getting Started

Fork this repo and clone into your local project to make use of the scripts here.  

### Prerequisites

The things you need before connecting to the repo.

* You need git installed on your VM
* And you need to request access to this repository if not already
* You need to generate a personal access token (PAT) if you want to make changes to this repository

## Usage

### As a code template for a new project

#### Fork the codebase repo:

Go to the lab organization's GitHub page and find the "codebase" repository.

Click the "Fork" button in the top right corner to create a personal copy of the repository under your GitHub account.

#### Create a new RStudio project linked to the forked repo:

Open RStudio and click "File" > "New Project" > "Version Control" > "Git".

Paste the URL of your forked "codebase" repository.

Choose a location for your project and click "Create Project".

#### Modify and commit changes locally:

Delete any scripts you don't need for your project. Modify existing scripts as needed for your analysis.
Create new scripts and files as required. Use Git commands within RStudio to track, commit, and review your changes:

```
Stage changes: git add <files>
Commit changes: git commit -m "Descriptive message"

```

#### Create a new remote repository for your project:

Go to your lab organization's GitHub page and click "New" to create a new repository.
Give it a descriptive name and choose appropriate settings (e.g., public or private).

#### Push your changes to the new remote repository:

In RStudio, go to "Git" > "Remotes" > "Add".

Enter a name for the remote (e.g., "origin") and paste the URL of your newly created repository.

Push your changes: git push -u origin master (assuming you're working on the "master" branch)

#### Continue working and collaborating:

Continue working on your project locally, making commits as needed.
Push your changes to the remote repository to share them with collaborators.
If others make changes to the main "codebase" repository, you can merge those changes into your project using Git commands.

### To add/modify code in the code_template repository

#### Fork it

Fork it first in github and give it a unique name eg code_template_David

#### Clone it

Clone the forked repo to your local machine

```
$ git clone https://github.com/DJMartino/code_templates_David.git

```

#### Branch off

Create a new branch to house your changes

```
$ git branch <newbranch>
$ git checkout <newbranch>

```

#### Make changes

Make and commit changes in the local repo. Test that they all work.

```
$ git add README.md
$ git commit

```

#### Push changes to the forked remote repo

Pushing changes to the forked remote repo will create a pull request in the main code base

```
$ git push origin <newbranch>

```
#### Make a pull request

On GitHub navigate to your forked repo and click "New pull request"

Choose the branches you made changes to the new branch and the branch you want to merge into <main/master>

Add descriptions for review. Once changes are reviewed the maintainers of the origial repo will incorporate
changes.

## Etiquette

Use clear and descriptive commit messages to track your work effectively.

Consider using branches for different features or experiments to keep your project organized.

Collaborate with your team members using pull requests to review and merge changes.

Refer to GitHub's documentation and online resources for more in-depth guidance on Git and GitHub workflows.

## Contributors

* David Martino
