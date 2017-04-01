---
layout: default
title: Setup Instructions
---

# Setup Instructions
*These instructions will help you setup your own version of Michael's project website.  Follow the instructions exactly*

## Boring Stuff
__Note:__ This section will focus on the installation of the project

You will need the following to run this project:

* Git
* Ruby
* Jekyll

Most modern computers come with Git installed. If you do not have it installed, you can download it at [https://git-scm.com/downloads](https://git-scm.com/downloads).

You will also need to download Ruby. Most modern Mac's come with Ruby pre-installed but if you do not have it, you can download it at [https://www.ruby-lang.org/en/downloads/](https://www.ruby-lang.org/en/downloads/). 

Installing Jekyll is very simple. To do that, you need to open a command prompt and type the following:

__Note__ - *Do not type the $ as it is a reminder that it is a command, to be entered on the command line.*

To clone the repository, type in the following: 

```bash
$ git clone https://github.com/michael-bateman/projects.michaelbateman.ca
```

Now, navigate to the directory by typing: 

```bash
$ cd projects.michaelbateman.ca
```

Now, you need to serve Jekyll to start the server: 

```bash
$ jekyll serve
```

Note: If you would like to serve the port on a different one than port 4000 type the following: 

```bash
$ jekyll serve --port <port_no>
```

## Customization
__Note:__ This section will focus on how to customize the website

Open the `projects` folder, and delete all contents.  The only thing that should be remaining is the empty folder.

Open the `projects.yml` file, which can be located in the `_data` directory.

Delete all lines of code except for lines 1-22

Now, you can customize that file for your projects.

To make a page for a project, make a new `.md` file in the `projects` directory.

The `YAML` front matter should be the following:

```ruby
---
layout: project
title: <title_of_website>
permalink: /<link_that_you_want_your_project_to_be_saved_to>/
project: <the_project_name>
---
```

It should now all work!