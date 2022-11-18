<h1>parallax scroll effects</h1>
<p>Scroll down to see this CSS property in action.</p>


<h2>So what is parallax scrolling, anyway?</h2>
<p>Parallax scrolling is a web design trend where the background image moves at a different speed than the foreground content whenever the user scrolls. While a strong effect can be created with JavaScript (i.e. by moving the background image slightly up while the user scrolls down, and vice-versa), a similar look and feel can also be achieved with pure CSS.</p>

<h2>How do we do it?</h2>
<p>To set things up, we need to start with a container that has some content inside of it (so that the user has something to scroll through). Next, we'll use the following CSS properties:</p>
<pre>
  <code>
    background-image: url('../img/parallax.webp');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  </code>
</pre>

<p>Now that we've set up our background image, as per usual, the following property will create the parallax effect:
</p>

<pre>
  <code>
    background-attachment: fixed;
  </code>
</pre>

<p>And that's it. All it takes is the <kbd>background-attachment</kbd> property.</p>
<p>Of course, all of these declarations can go into the background shorthand property to make our CSS a little neater and easier to manage:</p>

<pre>
  <code>
    background: url('../img/parallax.webp') center / cover no-repeat fixed;
  </code>
</pre>