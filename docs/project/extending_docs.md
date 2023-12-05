### Creating documentation

By default Browsedocs reads `readme.md` markdown file. If you have it by other names make sure to specify it in the `source` key in `.browsedocs.json` file.

```json
{
    ...
    "source": "documentation.md"
    ...
}
```

### Creating a multipage documentation

More often you would want to create a multipage documentation. Creating multipage documenation is simple. 

In your `.browsedocs.json` file add a key called `"sidebar"`

```py
{
    ...
    "sidebar":  [
        {
            "name": "Quick start", # display name of the heading you want
            "path": "documentation/index.md", # full path to the documentation
            "url": "quick-start/" # the display url you would like to have
        },
        {
            "name": "browsedocs.json",
            "path": "documentation/second-level/index.md",
            "url": "docs/browsedocs-json/"
        },
        ...
    ]
    ...
}
```

### updating your documentation

* Make the required changes in the documentation.
* On your profile click on my documentation.
* Click on update on the project card.

> Note If you made changes for a new version of your project make sure to update `"version"` key in `.browsedocs.json` file, else it will overwrite the existing version.

### Adding multiple versions

* Currently adding multiple versions can be acheived my making changes to `"version"` key in `.browsedocs.json` file