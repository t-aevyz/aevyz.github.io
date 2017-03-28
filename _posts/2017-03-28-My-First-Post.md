---
title: My First Post
date: 2017-03-28 01:26
categories: GitHub_Sites
series:  GitHub Sites For Beginner
show: true
---
# My First Post

Now that you have generated a site, you probably wish to actually post something on it.
### Writing Your First Post
You first want to write out your first post in Atom. Most posts that you shall write shall be posted in the `_posts` folder. Jekyll accepts posts in HTML or Markdown.

Markdown is a `Lightweight Markup Language`, in other words, it is used to format text. In the case of Jekyll, Markdown files are automatically converted into HTML webpages for you. This post is formatted using Markdown.

>#### For those with HTML Experience
For those with HTML experience, you are free to also include HTML snippets in your Markdown files. These will also be displayed on the site later, however it cannot be guaranteed to be bug free. You can also use the `include` method from Liquid, which shall be elaborated on in a further post.

### Creating the Post
Creating a post is very simple, in Atom simply Right Click the `_posts` folder and click on the `New File` option.

You must name your post in the following scheme:
`$YEAR-$MONTH-$DAY-$TITLE.md`

* `$YEAR` is the current **year** in **four** digit format
* `$MONTH` is the current **month** in **two** digit format
* `$DAY` is the current **date** in **two** digit format
* `$TITLE` is the **URL** of your post, make sure you use **hyphens** instead of spaces in your title.
* `.md` is your file extension for **M**ark**d**own files.
****


You can split the Markdown File into two parts, the `Front Matter` and the `Body`:

#### Front Matter
In the Front Matter, you can predefine variables, that shall be used to help create your site. The front matter **must** be the first thing in a post and must be valid and also **must** be enclosed in three hyphens, like this `---`.

The demo Markdown File provided with the theme has the following Front Matter:
>```
>---
>title: What is this, anyway?
>date: 2013-12-08 19:55:16
>categories: jekyll testing
>---
>```

By default, this theme requests you to use the following tags:
* `title: ` gives the title of the page, and what shall later also appear at the top of every page, as well as what shall be considered by the browser as a page title.
* `date: ` is where you shall list the current date in a `YYYY-MM-DD-HH-MM-SS` format, so that the site is able to sort your posts chronologically.
* `categories: ` is used for sorting purposes, as it allows you to find posts of the same type. Depending on the configuration of your website, this may alter the domain. By default Jekyll gives each post the following URL: `/:categories/:year/:month/:day/:title.html`.

If you want to read more about this, you can do so at the [official Ruby Docs on Front Matter](https://jekyllrb.com/docs/frontmatter/). At a latter point, we shall be adding our own variables to the Front Matter, but for now, these shall do.

#### The Text Body
In the text body you are free to post whatever you want. You are free to use Markdown or HTML in this section. Furthermore, you can use the Liquid Template Language, which will shall elaborate on in another post.

Your best bet in understanding Markdown is to simply read the [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet), as it explains the formatting in a far better way then I could.
