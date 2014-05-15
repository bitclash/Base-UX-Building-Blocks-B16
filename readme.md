# UXE - Base UX Building Blocks

For this assignment, students will be required to leverage concepts like Style Tiles, Flow Documents and Wireframes to convey project intent.



## Assignment description

- Style Tile
  - This assignment is the first in preparation for the first Project week.
  - Using either an existing design or coming up with a custom design, working with a partner, the goal of this assignment is to create a Style Tile that will be the design foundation for your project.
  - This Style Tile should contain the following common features:
    - Logo
    - Color palette
    - Possible textures
    - Conceptual adjectives
    - Typography
    - Button treatments
    - Possible background treatments
    - Use versioning
- Flow diagram
  - Building a flow diagram is a thought intensive process. Using design/visual tools can sometimes cloud over the real thought process. Using a DOT file, you can think through the process of anything; your daily routine, how you get to school or making a sandwich.
  - The goal of this assignment is to get used to using this type of pseudo code tool to think through an algorithmic process. Make sure to include decision points and alternative endings.
- Informational Architecture (wireframe)
  - Using wireframes for IA is an effective tool for communicating concepts of layout with a client as this keeps the discussion focused on the items at hand. Wireframes are quick to create, easy to modify and have little emotional connection.
  - For this assignment, I want you to create IA wireframes for an online web app that addresses this scenario:
    - The app you are working on is an emergency contact form where the user (victim) is the owner of private property that has been vandalized.
    - The user requires your service to address the situation, but may or may not be a registered user or previous customer.
    - The user requires an interface that will either directly address or link to:
      - instructions about the the service
      - login/registration services
      - navigation to related information
      - navigation to company related information
      - additional products and services
      - emergency chat option
      - general contact
    - A registered user requires a form to log the vandalizem with your service
      - location of the issue
      - description of property and hard materials (e.g. brick, class, etc ...)
      - upload photo(s) of the damage
      - contact information
        - person of contact
        - phone number
        - email address
      - Schedule onsite estimation



## Submitting assignments

Submitting assignments for this course will require leveraging some of the more advanced features of Github. These features will not only improve your knowledge of Git and Github, but also provide practice exercises for working on a distributed project with a large team.

## How to submit an assignment

In order to submit assignments, please use the following steps

1. [Fork this repo][1] so that you have a working version
1. [Clone the forked repo][2] to your local computer
1. Create a folder named with your name, example `dale-sande`
1. Once completed with your assignment, commit code to the master branch and push to Github `git push origin master`
1. From __your fork__ of the project, initiate a pull request to the parent repo

## Assignment review

When a pull request is initiated, I will be notified of the update and comment on the submitted assignment via Github tools.

## Keeping your local repo up to date
Your local repo will be an independent version of the original repo from the moment you fork the repo. In order to keep your local repo up to date with the original repo, you need to do what is called an [upstream pull][3].

To manage an upstream pull, I suggest updating your `.bash_profile` and your `.gitconfig` file with easy to remember aliases.

### .bash_profile

In your `.bash_profile` add the following alias

```
alias upstream="git remote add upstream \$@"
```

From the command line you simply need to refer to the alias and add the path to the upstream repo as shown in the following example.

```
$ upstream https://github.com/blackfalcon/unicorn-class-css-section.git
```

Once the upstream repo is configured for your local repo, this never needs to be reset again, unless you delete your local repo.

### .gitconfig
In your `.gitconfig` add the following alias

```
pu = !"git fetch origin -v; git fetch upstream -v; git merge upstream/master"
```

From the command line, within the project repo, enter the following command to pull latest code from the upstream master.

```
git pu
```




[1]:https://help.github.com/articles/fork-a-repo
[2]:https://help.github.com/articles/fork-a-repo#step-2-clone-your-fork
[3]:https://help.github.com/articles/syncing-a-fork
