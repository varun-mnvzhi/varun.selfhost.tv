---
# `parent-C.md` is a parent page in the website

# `title` sets the title of the web page
# appears at the beginning of the web page and in the tab of web browsers
title: Contact Me
# `description` is a tag line or sub-heading for the web page.
description:
# `type` decides what kind of page is this and where does it appear
# set this to `parent` to make this page appear in the navigation bar
# set this to the `title` of the parent you want it to appear under
type: parent
# `order` decides order of appearance of this web page in the navigation bar
# set this to `1` for the homepage (`index.md`)
order: 5
# `layout` is the looks of this web page
# set this to `parent` for everything that is listed in the navigation bar
# set this to `child` for everything that is not listed in the navigation bar
layout: parent
---

[//]: # (Here you can write the content of the page in markdown.)

{:md_center: style="text-align: center;"}
Reach out to me and let's create something amazing together.
{: md_center}

<div class="row">
  <div class="offset-by-two eight columns">
    <form class="cf">
      <div class="half left cf">
        <input type="text" id="input-name" placeholder="Name">
        <input type="email" id="input-email" placeholder="Email address">
        <input type="text" id="input-subject" placeholder="Subject">
      </div>
      <div class="half right cf">
        <textarea name="message" type="text" id="input-message" placeholder="Message"></textarea>
      </div>
      <input class="button button-primary" type="submit" value="Submit" id="input-submit">
    </form>
  </div>
</div>