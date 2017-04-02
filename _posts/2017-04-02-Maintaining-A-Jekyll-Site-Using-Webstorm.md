---
layout: post

title:  Maintaining A Jekyll Site Using Webstorm

date: 2017-04-02 16:52

categories: GitHub_Sites

series:  A Non-Programmers Guide To GitHub Sites

---
Whilst WebStorm is a powerful IDE focused on websites, it does not directly support Jekyll, however using certain plugins, it is able to perform a lot of functions that make creating Jekyll sites far easier, such as integrated Git to allow for easier uploading to GitHub sites.

Note however that [WebStorm](https://www.jetbrains.com/webstorm/whatsnew/) is not free for the general public, however offers discounts or complimentary lisences to certain groups, including university students and open source contributors.

As this is slightly longer than my regular post, I shall be using a table of contents to help formatting.

### Cloning a Project in WebStorm
Simply Navigate to `VCS > Checkout from Version Control > GitHub`. There you shall be prompted to generate a connection to your GitHub account, assuming you haven't already once logged into the system before.

A popup shall appear, asking which repository you wish to clone and where it should be cloned to.

![Choose which repo to clone dialog](/images/adv-tut/clone-from-github.png "Select Which Repo You Wish To Clone")

With that, your project should have opened in Webstorm.

### Installing the Markdown Plugin
By default, Webstorm does not support Markdown. Therefore we need to get a plugin to do so. Navigate to `Settings > Plugins > Browse Repositories`.

![Plugins: Browse Repositories](/images/adv-tut/settings-plugins.png)

In the following window search for `Markdown Navigator` and install it.

![Install Navigator Plugin](/images/adv-tut/markdown-navigator-plugin.png)

Once you've installed the plugin, you shall be propted to restart WebStorm. Upon restart, you shall have a preview on the right hand side when typing out Markdown texts.

![Example of Markdown Plugin](/images/adv-tut/example-markdown-plugin.png)

### Creating a Template
Something that will speed up the writing of posts, is if you can automatically generate your front matter. This can be done in the form of templates.

>Reminder:
><br>The Front Matter (the YAML header) of the Markdown post is not in the Markdown format, but in YAML, however the Markdown plugin reads the entire document as Markdown, thus formatting may look strange.
><br>My personal tip would be to use double line breaks between each item in the header, so that Markdown thinks you are trying to continue writing on the next line. Furthermore, you should also add a line break before the closing `---`, as it prevents the formatting from messing up in the preview.