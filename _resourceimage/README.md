# Adding an image

To add an image:

1. [create a new file within the _resourceimage folder](https://github.com/maban/styleguides/new/gh-pages/_resourceimage) (the same one as this README). 
2. Give it a name that's the same as the title of the image, with words separated by hyphens, with .md at the end.
3. Paste the following templating code into it:

```
---
title: Title of image
link: A static link to the image
author: The author's name
site: The site that the linked image is published on
---

An optional short description of the image goes here
```

The text sandwiched between the --- --- is called "YAML front matter" and this takes the data and inserts it all into the template. The bit after that is the actual content.

**Do not add any links to the content** because the whole thing is wrapped in a link tag, so adding another link will stop it working.

## Example

Here's an example of an image I've added to the _resourceimage folder:

```
---
title: Lorem Pizza
link: http://lorempizza.com
author: rlemon
site: http://github.com/rlemon
---

A quick and simple service for getting pictures of pizza for use as placeholders in your designs or code. Just put your image size (width & height) after our URL and you'll get a placeholder.

_Max image size restricted to 1920 x 1080_

## Examples

![Lorem Pizaa 380x240 example 1](http://lorempizza.com/380/240)
`http://lorempizza.com/380/240`

![Lorem Pizaa 380x240 example 2](http://lorempizza.com/i/380/240)
`http://lorempizza.com/i/380/240`
```
