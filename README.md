commentcava
===========

what is commentcava?
-------------

commentçava is a comment system in javascript for static websites (ie. Jekyll). It is powered by Ajax &amp; a SQlite database and contains a captcha to avoid flood.
It should work with multiple domains (crossdomains) too, but i haven't tested it.

How to use it?
-------------
Copy files on your webserver.

Then, configure commentcava.js corresponding to your domain/subdomain/subfolder
```javascript
	var gurl = "http://example.com/commentcava.php";
```

Finally, edit every webpage you want to display comments as following:

add this to &lt;head&gt; or before &lt;/body&gt; :

```html
    <script src="jquery.min.js" type="text/javascript"></script>
    <script src="commentcava.js" type="text/javascript"></script>
```

add this part where you wants comments (on a post page) :

```html
    <div id="comments" class="comments">
      <img src="loading.gif" alt="Loading comments…"/>
    </div>
```

commentcava provides a default css, but if you don't like it, make another one :).

Why create commentcava?
-------------

I started it for a friend, then told me i could reuse it.
I created it so it is the simplest possible, sticks to 2 methods: 1) retrieve comments 2) post comments
For security i added a captcha on the form to post a comment.
I know some alternatives exists on the web, like jskomment, but i consider it is overkill to use it.

BONUS: what does commentcava means and how to pronounce?
-------------

the french «Comment ça va?» is the equivalent of the english «How are you?»
I found this fun when searching for a name containing "comment".

How to pronounce it?
Comment: /kɔ.m&atilde;/
ça     : /sa/
va     : /va/