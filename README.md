# HTML Boilerplate
![HTML](https://images.unsplash.com/photo-1603969072881-b0fc7f3d77d7?q=80&w=3540&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

## Introduction

All HTML documents have the same basic structure or boilerplate that needs to be in place before anything useful can be done. In this lesson, we will explore the different parts of this boilerplate and see how it all fits together.

## Lesson overview

This section contains a general overview of topics that you will learn in this lesson.

* How to write the basic boilerplate for an HTML document.
* How to open HTML documents in your browser.

## Creating an HTML file

To demonstrate an HTML boilerplate, we first need an HTML file to work with.

Create a new folder on your computer and name it **html-boilerplate**. Within that folder create a new file and name it **index.html**.

You’re probably already familiar with a lot of different types of files, for example doc, pdf, and image files.

To let the computer know we want to create an HTML file, we need to append the filename with the **.html** extension, as we have done when creating the **index.html** file.

It is worth noting that we named our HTML file **index**. We should always name the HTML file that will contain the homepage of our website **index.html**. This is because web servers will by default look for an index.html** page when users land on our websites – and not having one will cause big problems.

## The DOCTYPE

Every HTML page starts with a doctype declaration. The doctype’s purpose is to tell the browser what version of HTML it should use to render the document. The latest version of HTML is HTML5, and the doctype for that version is `<!DOCTYPE html>`.

The doctypes for older versions of HTML were a bit more complicated. For example, this is the doctype declaration for HTML4:

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

However, we probably won’t ever want to be using an older version of HTML, so we’ll always use `<!DOCTYPE html>`.

Open the **index.html** file created earlier in your text editor and add `<!DOCTYPE html>`to the very first line.

## HTML element

After we declare the doctype, we need to provide an `<html>` element. This is what’s known as the root element of the document, meaning that every other element in the document will be a descendant of it.

This becomes more important later on when we learn about manipulating HTML with JavaScript. For now, just know that the `<html>` element should be included on every HTML document.

Back in the **index.html** file, let’s add the `<html>` element by typing out its opening and closing tags, like so:
```
<!DOCTYPE html>
<html lang="en">
</html>
```
Noticed the word `lang` here? It represents an HTML attribute which is associated with the given HTML tag i.e. `<html>`in this case. These attributes provide additional information about HTML elements. (More about **HTML attributes** in the following lesson.)

### What is the lang attribute?

`lang` specifies the language of the text content in that element. This attribute is primarily used for improving accessibility of the webpage. It allows assistive technologies, for example screen readers, to adapt according to the language and invoke correct pronunciation.

## Head element

The `<head>` element is where we put important meta-information **about** our webpages, and stuff required for our webpages to render correctly in the browser. Inside the `<head>`, we **should not** use any element that displays content on the webpage.

Back in our **index.html** file, let’s add a `<head>` element with a `<meta> `element and a title within it. The` <head>` element goes within the` <html>` element and should always be the first element under the opening `<html>` tag:
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>My First Webpage</title>
  </head>
</html>
```
### Meta element

We should always have the `<meta>` tag with the charset encoding of the webpage in the `<head>` element: `<meta charset="UTF-8">.`

Setting the encoding is very important because it ensures that the webpage will display special symbols and characters from different languages correctly in the browser.

### Title element

Another element we should always include in the head of an HTML document is the `<title>` element:

`<title>`My First Webpage`</title>`

The `<title>` element is used to give webpages a human-readable title, which is displayed in our webpage’s browser tab. For example, if you look at the current tab’s name of your browser, it will read “HTML Boilerplate | The Odin Project”; this is the `<title>` of the current **.html** file.

If we didn’t include a `<title>` element, the webpage’s title would default to its file name. In our case that would be **index.html**, which isn’t very meaningful for users; this would make it very difficult to find our webpage if the user has many browser tabs open.

There are many more elements that can go within the head of an HTML document. However, for now it’s only crucial to know about the two elements we have covered here. We will introduce more elements that go into the head throughout the rest of the curriculum.

Body element

The final element needed to complete the HTML boilerplate is the `<body>`element. This is where all the content that will be displayed to users will go - the text, images, lists, links, and so on.

To complete the boilerplate, add a `<body> `element to the **index.html** file. The `<body>` element also goes within the` <html>` element and is always below the `<head>` element, like so:
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>My First Webpage</title>
  </head>

  <body>
  </body>
</html>
```

For more information about **HTML Boilerplate** check out the MDN docs.[MDN](https://www.theodinproject.com/lessons/foundations-html-boilerplate)