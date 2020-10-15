
# Intro to Markup and Web Design

**Work to have done**: Try and relax!

**Plan for the day**:

1. Introduction to markup languages (30ish min)
2. Web-design unit overview and assignment (10 min)
3. Tour of unit resources (5-10 min)
4. Start the homework during class <!-- so we can make sure you've got Atom working properly -->

## 1. Introduction to Markup Languages (10-15 min)

### Begin with a breath
Our next unit takes us into the world of hypertext, a more interactive medium. Before we dive in deep, <strong>come with me to the <a href="http://www.csszengarden.com">CSS Zen Garden</a></strong>.

Some things to notice:

* Responsive design: the same page can change appearance to suit the "viewscreen" (especially as the width changes).

<!-- demo Verde Moderna (the default), -->

* The visual hierarchy holds here, too – including uses of negative space as a way of establishing rhythm.

<!-- Screen Filler, -->

* So, too, are we retaining the importance of color schemes for both coherence and contrast.

<!-- Mid-Century Modern -->

* This is all _exactly_ the same html.

<!-- Even A Robot Named Jimmy. -->

### Markup: separating content from display
How?

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>acronym</th>
      <th>stands for</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>HTML</td>
      <td>HyperText Markup Language</td>
    </tr>
    <tr>
      <td>CSS</td>
      <td>Cascading Style Sheets</td>
    </tr>
  </tbody>
</table>

What does that mean??

Per [the tutorial I'm assigning you for homework](https://internetingishard.com/html-and-css/introduction#html-css-and-javascript),
> HTML is for adding meaning to raw content by marking it up.
CSS is for formatting that marked up content.

<!-- Make the connection to their own markup on the Issue Queue: bold, italic, etc. Make the connection to -->

In other words:

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>acronym</th>
      <th>stands for</th>
      <th>used for</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>HTML</td>
      <td>HyperText Markup Language</td>
      <td>content, groupings</td>
    </tr>
    <tr>
      <td>CSS</td>
      <td>Cascading Style Sheets</td>
      <td>display / presentation</td>
    </tr>
  </tbody>
</table>

There are other languages that interact with these two, especially JavaScript, but also PHP and Python and Ruby: they can dynamically generate or change the HTML and CSS. And there are preprocessor languages that make it easier to generate HTML and CSS on your own: Markdown, the syntax you use in GitHub READMEs and forum posts, is essentially a shortcut form of HTML. But HTML and CSS are the core of what gets shown on the screen.

Let's take Markdown as an example:

* If you want to make something bold, you...
  - put `**asterisks**` on either side of it.
* If you want italics, you...
  - put `_underscore_` on either side (single asterisks will work, too).

<div class="alert alert-info">
The basic idea is that you need to signal where the <em>marked-up text</em> begins and ends.
</div>

The same is true in HTML, but it looks a little different:

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>what we’re marking</th>
      <th>Markdown syntax</th>
      <th>HTML syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>strong text</td>
      <td><code class="language-plaintext highlighter-rouge">**surrounding asterisks**</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;strong&gt;opening and closing tags&lt;/strong&gt;</code></td>
    </tr>
    <tr>
      <td>emphasized text</td>
      <td><code class="language-plaintext highlighter-rouge">_surrounding underscore_</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;em&gt;opening and closing tags&lt;/em&gt;</code></td>
    </tr>
  </tbody>
</table>

<div class="alert alert-info">
<p>Unlike in Markdown, opening and closing tags in HTML aren't exactly the same. But they're <em>almost</em> the same: a closing tag in HTML just adds the slash after the first angle bracket.</p>

<p>You can think of them as being like <a href="https://xkcd.com/859/">parentheses</a>: In general, every HTML tag you open should close. (You can nest a complete pair of tags inside another pair (like these parentheses), but you can't close the outer pair before closing the inner pair without causing problems.)</p>
</div>

One nice thing about having the tags themselves marked by angle brackets is that you can add information to them:

<table class="table table-bordered thead-light">
  <thead>
    <tr>
      <th>what we’re marking</th>
      <th>Markdown syntax</th>
      <th>HTML syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>a basic hyperlink</td>
      <td><code class="language-plaintext highlighter-rouge">[anchor text](http://destination)</code></td>
      <td><code class="language-plaintext highlighter-rouge">&lt;a href="http://destination"&gt;anchor text&lt;/a&gt;</code></td>
    </tr>
    <tr>
      <td>a hyperlink with extra info</td>
      <td><em>no default way to do it!</em></td>
      <td><span title="title text is what you see on hover"><code class="language-plaintext highlighter-rouge">&lt;a href="http://destination" class="dummylink external" title="Explanation of where link goes"&gt;anchor text&lt;/a&gt;</code></span></td>
    </tr>
  </tbody>
</table>

### A Demo
Some of this is easier to understand with a live demo! Let's head over to a [CodePen](https://codepen.io/benmiller314/pen/poJROZM?editors=1100) where we can get some instant results from adding new HTML and CSS rules.

<!--
CSS rules to hit:
1. headers
2. paragraphs
3. using Atom to auto-close tags
4. no default spacing: let's change it!
5. a div is like a layer-group: collect these things, operate on them together. it's a container.
6. ids and # selectors
7. classes and . selectors
 -->


## 2. Web-design unit overview and assignment (10 min)

As I explained in the syllabus, your third project is to **build a portfolio website using basic html and css files** — as opposed to a site manager like WordPress or Wix — **along with any media assets you wish to embed.** In assigning this, I have two main goals for you:

1. to learn how to manage a composite project made up of multiple interlinking files, and
2. to explore the affordances of the web design stack as a medium, and especially its ability to _flexibly render content for multiple audiences or reading priorities_.

<div class="alert alert-success">
  To read the full assignment – and fork a copy for yourself – go to <strong><a href="https://github.com/benmiller314/website-portfolio-2020spring#project-3-website-portfolio">github.com/benmiller314/website-portfolio-2020spring</a></strong>.
</div>

Let's read through this together.

<!-- Go through overview, constraints, deadlines. -->

## 3. Tour of unit resources

I just want to give you a quick overview of the assets and advice I've compiled so far on [the course site's resources page]({{site.github.url}}/resources).

<div class="alert alert-info">
If you find yourself breezing through the Interneting is Hard tutorial, you can find other self-paced learning opportunities here.
</div>

## Homework for Next Time

* **Do** as much of the [Interneting is Hard (but it doesn't have to be)](https://internetingishard.com/html-and-css/) tutorial as time and interest allow – but *at least parts 1-4* (from "Introduction" through "Hello, CSS")
* **Show your work** by pushing your tutorial code to GitHub.
   - I've already created folders for parts 1-3 in the GH repo you just forked; clone it to your local computer, and you should be able to work in those folders and push.
   - But note that _you'll need to add your own folder_ for part 4, and thereafter.

<div class="alert alert-info">
Let's get started in class, so I can be available for Q&A – especially if you're still getting used to Atom!
</div>

<div class="alert alert-warning">
To get credit for asynchronous participation, play around in the <a href="https://codepen.io/benmiller314/pen/poJROZM?editors=1100">demo CodePen</a> and take some screenshots to show me what's changed; send these to me by email, along with any questions. Then just get started on that tutorial for homework...
</div>