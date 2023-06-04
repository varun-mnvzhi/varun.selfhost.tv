---
# `parent-C.md` is a parent page in the website

# `title` sets the title of the web page
# appears at the beginning of the web page and in the tab of web browsers
title: Contact Me
# `description` is a tag line or sub-heading for the web page.
description: I dabble in Genre C
# `type` decides what kind of page is this and where does it appear
# set this to `parent` to make this page appear in the navigation bar
# set this to the `title` of the parent you want it to appear under
type: parent
# `order` decides order of appearance of this web page in the navigation bar
# set this to `1` for the homepage (`index.md`)
order: 5
# `layout` is the looks of this web page
# set this to `parent` for everything that is listed in the navigation bar
# set this to `default` for everything that is not listed in the navigation bar
layout: parent
---

[//]: # (Here you can write the content of the page in markdown.)

Reach out to me and let's create something amazing together.

<h2>Drop me an email</h2>
<form class="cf">
  <div class="half left cf">
    <input type="text" id="input-name" placeholder="Name">
    <input type="email" id="input-email" placeholder="Email address">
    <input type="text" id="input-subject" placeholder="Subject">
  </div>
  <div class="half right cf">
    <textarea name="message" type="text" id="input-message" placeholder="Message"></textarea>
  </div>  
  <input type="submit" value="Submit" id="input-submit">
</form>





@import "compass/css3";

@import url(https://fonts.googleapis.com/css?family=Merriweather);
$red: #e74c3c;

*, 
*:before, 
*:after {
   @include box-sizing(border-box); 
}

html, body {
  background: #f1f1f1;
  font-family: 'Merriweather', sans-serif;
  padding: 1em;
}

h1 {
   text-align: center;
   color: #a8a8a8;
   @include text-shadow(1px 1px 0 rgba(white, 1));
}

form {
   max-width: 600px;
   text-align: center;
   margin: 20px auto;
  
  input, textarea {
     border:0; outline:0;
     padding: 1em;
     @include border-radius(8px);
     display: block;
     width: 100%;
     margin-top: 1em;
     font-family: 'Merriweather', sans-serif;
     @include box-shadow(0 1px 1px rgba(black, 0.1));
     resize: none;
    
    &:focus {
       @include box-shadow(0 0px 2px rgba($red, 1)!important);
    }
  }
  
  #input-submit {
     color: white; 
     background: $red;
     cursor: pointer;
    
    &:hover {
       @include box-shadow(0 1px 1px 1px rgba(#aaa, 0.6)); 
    }
  }
  
  textarea {
      height: 126px;
  }
}


.half {
  float: left;
  width: 48%;
  margin-bottom: 1em;
}

.right { width: 50%; }

.left {
     margin-right: 2%; 
}


@media (max-width: 480px) {
  .half {
     width: 100%; 
     float: none;
     margin-bottom: 0; 
  }
}


/* Clearfix */
.cf:before,
.cf:after {
    content: " "; /* 1 */
    display: table; /* 2 */
}

.cf:after {
    clear: both;
}