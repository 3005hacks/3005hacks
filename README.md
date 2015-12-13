# 3005hacks.github.io

This repository houses the homepage of 3005hacks. Check it out live [here](http://3005hacks.com).

## Structure
```
|-- _data/ (data that appears in the website)
    \
    |-- contact.yml  ()
    |-- members.yml  ()
    |-- projects.yml  ()
|-- _includes/
    \
    |-- footer.html
    |-- header.html
    |-- scripts.html
    
|-- README.md (This file)
|-- density/
    \
    |-- density.py  (the executable for this application)
    |-- static/     (your static files, such as js, css, imgs)
    |-- tests/
```

## Updating the site
Data, like projects, members, and links, lives in the `_data/` directory. The purpose of this structure is to allow information to be easily updated without having to dive into the raw HTML.

### Adding a new project
Projects are found in `_data/projects.yml`. Each project has the following properties:
- __name__
- __image:__ Images should be square.
- __alttext:__ Alt text is a short description of the image appears in that project’s `<img>` tag. It’s important for accessibility on the web.
- __link:__ Link to the project live online

To add a new project, simply create a new block with these parameters. Note that a hyphen (`-`) only appears once for each project in front of its name. The other properties are simply added on a new line.

### Adding a new member
Members are found in `_data/members.yml`. Each member has the following properties:
- __name__
- __description:__ A short paragraph about the member, appears under their photo on the site.
- __image:__ Images should be square.
- __alttext:__ Alt text is a short description of the image appears in that member’s `<img>` tag. It’s important for accessibility on the web.
- __twitter__ (optional)
- __github__ (optional)
- __linkedin__ (optional)

To add a new member, simply create a new block with these parameters. Note that a hyphen (`-`) only appears once for each member in front of his or her name. The other properties are simply added on a new line.

### `contact.yml`
`contact.yml` includes links that appear in the contact portion of the website. This file contains the 3005hacks email address and GitHub organization. Any other links that appear in the contact portion should be added here.
