<p align="center">
  <img src="https://raw.githubusercontent.com/michu1234/Goel/master/src/img/goel_background.jpg" width="100%" alt="Goel logo">
</p>

# PLACEHOLDER

> Sass has a special kind of selector known as a “placeholder”. It looks and acts a lot like a class selector, but **it starts with a % and it's not included in the CSS output**. In fact, any complex selector (the ones between the commas) that even contains a placeholder selector isn't included in the CSS, nor is any style rule whose selectors all contain placeholders,
<br />


```scss
// placeholders
%purple {
  color: purple;
}
%red {
 color: red;
}

p {
  @extend %purple;
}

span {
  @extend %purple;
}

h2 {
  @extend %purple;
}

h1 {
  @extend %purple;
}

```
<p style="font-size: 55px" align="center">👇</hp>

```scss
h1, h2, span, p {
  color: purple;
}

```
&nbsp;

<h6 align="center">I would like to show you my approach to writing clean and developer friendly SCSS architecture. This is the way I would like to think about it nowadays.</h6>
&nbsp; &nbsp;

<p align="center"><img src="https://github.com/michu1234/Goel/blob/master/src/img/goel_logo.jpg?raw=true" width="50px" alt="Goel logo"> </p>
<h5 align=center>GOEL  - Utility SASS Placeholders</h5>
<p align="center">GOEL is a SCSS library, which consists of multiple placeholders, build in utility / functional / atomic style.</p>
&nbsp; 
&nbsp;
This approach comes with multiple benefits for front-end / ui developers.

- match semantic and functional css
- create developer friendly class names using well known methodologies like BEM, OOCSS
- use well known architecure like ITCSS
- write clean CSS without unnecesery repetition
- write clean HTML without cluttering it with unnecessary classes
- stop wasting time for setup additional dependencies like purgeCSS: **unused placeholders are not included in output!**

&nbsp;
Below you can find materials, that were very inspiring for:

&nbsp;

## Code comparison

<p align="center"><img width="100%" src="https://raw.githubusercontent.com/michu1234/Goel/master/src/img/goel_comparison.jpg" alt="goel comparison code" border="0"></p>

## Create files and folders

The file explorer is accessible using the button in left corner of the navigation bar. You can create a new file by clicking the **New file** button in the file explorer. You can also create folders by clicking the **New folder** button.

## Switch to another file

All your files and folders are presented as a tree in the file explorer. You can switch from one to another by clicking a file in the tree.

## Rename a file

You can rename the current file by clicking the file name in the navigation bar or by clicking the **Rename** button in the file explorer.

## Delete a file

You can delete the current file by clicking the **Remove** button in the file explorer. The file will be moved into the **Trash** folder and automatically deleted after 7 days of inactivity.

## Export a file

You can export the current file by clicking **Export to disk** in the menu. You can choose to export the file as plain Markdown, as HTML using a Handlebars template or as a PDF.


# Synchronization

Synchronization is one of the biggest features of StackEdit. It enables you to synchronize any file in your workspace with other files stored in your **Google Drive**, your **Dropbox** and your **GitHub** accounts. This allows you to keep writing on other devices, collaborate with people you share the file with, integrate easily into your workflow... The synchronization mechanism takes place every minute in the background, downloading, merging, and uploading file modifications.

There are two types of synchronization and they can complement each other:

- The workspace synchronization will sync all your files, folders and settings automatically. This will allow you to fetch your workspace on any other device.
	> To start syncing your workspace, just sign in with Google in the menu.

- The file synchronization will keep one file of the workspace synced with one or multiple files in **Google Drive**, **Dropbox** or **GitHub**.
	> Before starting to sync files, you must link an account in the **Synchronize** sub-menu.

## Open a file

You can open a file from **Google Drive**, **Dropbox** or **GitHub** by opening the **Synchronize** sub-menu and clicking **Open from**. Once opened in the workspace, any modification in the file will be automatically synced.




# Publication

Publishing in StackEdit makes it simple for you to publish online your files. Once you're happy with a file, you can publish it to different hosting platforms like **Blogger**, **Dropbox**, **Gist**, **GitHub**, **Google Drive**, **WordPress** and **Zendesk**. With [Handlebars templates](http://handlebarsjs.com/), you have full control over what you export.

> Before starting to publish, you must link an account in the **Publish** sub-menu.

## Publish a File

You can publish your file by opening the **Publish** sub-menu and by clicking **Publish to**. For some locations, you can choose between the following formats:

- Markdown: publish the Markdown text on a website that can interpret it (**GitHub** for instance),
- HTML: publish the file converted to HTML via a Handlebars template (on a blog for example).

## Update a publication

After publishing, StackEdit keeps your file linked to that publication which makes it easy for you to re-publish it. Once you have modified your file and you want to update your publication, click on the **Publish now** button in the navigation bar.

> **Note:** The **Publish now** button is disabled if your file has not been published yet.

## Manage file publication

Since one file can be published to multiple locations, you can list and manage publish locations by clicking **File publication** in the **Publish** sub-menu. This allows you to list and remove publication locations that are linked to your file.


# Markdown extensions

StackEdit extends the standard Markdown syntax by adding extra **Markdown extensions**, providing you with some nice features.

> **ProTip:** You can disable any **Markdown extension** in the **File properties** dialog.


## SmartyPants

SmartyPants converts ASCII punctuation characters into "smart" typographic punctuation HTML entities. For example:

|                |ASCII                          |HTML                         |
|----------------|-------------------------------|-----------------------------|
|Single backticks|`'Isn't this fun?'`            |'Isn't this fun?'            |
|Quotes          |`"Isn't this fun?"`            |"Isn't this fun?"            |
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|




## UML diagrams

You can render UML diagrams using [Mermaid](https://mermaidjs.github.io/). For example, this will produce a sequence diagram:

