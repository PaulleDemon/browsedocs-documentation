### Introduction

A project is a useful tool or library created by an individual or collective collabrators. A Project name remains the same for most of the life time of the project.

### Creating Project
To create a project, first make sure you have logged in. 

* Once you have logged in click on your profile on the top right corner.

* You will see a dropdown, click on create Documentation

<p align="center">
    <img src="https://github.com/PaulleDemon/browsedocs-documentation/blob/main/images/create-doc.png" alt="create doc" style="max-width: 150px;">
</p>

* Now import your desired project.
<p align="center">
    <img src="https://github.com/PaulleDemon/browsedocs-documentation/blob/main/images/select-repo.png" alt="create doc" style="max-height: 150px;">
</p>

* Ensure your repository has readme.md or someother documenation file.

* Once you import by default you will see readme.md as your default documentation file, you can change this using `.browsedocs.json` file.

* fill in the appropriate fields and click on save at the bottom.

<p align="center">
    <img src="https://github.com/PaulleDemon/browsedocs-documentation/blob/main/images/create-project.png" alt="create doc" style="max-height: 250px;">
</p>

* Thats it your project is created, once your documenation is ready you'll receive an email.

### .browsedocs.json file

`.browsedocs.json` file is a configuration file where you can define the version, source, add additional details about the project.

To get started start by adding the `.browsedocs.json` file in the root folder.
Some of the configurations are as listed below

```py
{
    "version": "1.0.0",
    "unique_name": "browsedocs", # choose a unique name
    "project_name": "browsedocs",
    "about": "This is a simple and  about section for browsedocs. You can make it multiline by using the \n character: \n example1 \n example2",
    "source": "docs/",  #  add the path to the documentation if its a file write the path to the file. If its a folder just add path to that folder.
    
    "source_code": "https://github.com/PaulleDemon/browsedocs",
    
    "doc_type": "pgm-lng", # if your documentation is related to programming language give "pgm-lang" as value else "tool" as the value.
    
    "project_logo": "https://github.com/PaulleDemon.png", # project logo url (optional)

    "additional_links": { # optional
        "Examples": "https://github.com/PaulleDemon/browsedocs" # max two links
    },
    "authors": ["Paul"], # list of authors
    "tags": "python, documentation",
    "sponsor": { # optional
        "github": "PaulleDemon",
        "patreon": "username",
        "opencollective": "username",
        "buymeacoffee": "artpaul",
        "paypal": "paypal.me username",
    },
    "social":{ # optional
        "stackoverflow": "tkvideoplayer", # add the stackoverflow tag
        "reddit": "reddit", # reddit community name
        "twitter": "twitter", # twitter username
        "discord": "discord", # discord community name
        "mastodon": "mastodon", # mastodon username
    }
}
```

> Note: the comments are added for your understanding. Json files don't accept comments.

### sharing your documentation

* Short url: you can paste the unique_id after the `browsedocs.com`, it will look something along `bWXP7P4Tpxhz` so example: https://browsedocs.com/bWXP7P4Tpxhz/
* The shortened url can be retrieved either from your email or from the url of the documentation