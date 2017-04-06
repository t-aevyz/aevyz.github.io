                                            
---
layout: post

title:  Customizing The Projects Page

date: 2017-04-04 22:11

categories: GitHub_Sites

series:  A Non-Programmers Guide To GitHub Sites

---

The Projects Page comes by default with some sliding panels, however not all of the features on the page are functional when forked.

## Non-Working Features
The default copy of the site can be found [here](https://aevyztutorial.github.io/herring-cove-original/projects.html
).

As you can tell, Photography and Coding Buttons do not work. Furthermore the Lorem Ipsum must be replaced with your actual project descriptions.

## Replacing Text

One of these text containers is created using the following code.

```
<div class="container">
  <div class="project-box">
    <div class="row">
      <div class="col-md-3 project-image">
        <img src=" -->Add a url to a picture here<-- " style="max-width: 145px;">
      </div>
      <div class="col-md-9 project-post">
        <h1>-->Title<--</h1>
        <h4>-->Subtitle<--</h4>
        <p class="meta"><small>&nbsp;<i class="fa fa-calendar-o"></i> -->This Posts Year<-- </small></p><hr/>
        <div class="post">

        -->Your Content Goes Here<--

        </ul>
        </div>
      </div>
    </div>
  </div>

```
