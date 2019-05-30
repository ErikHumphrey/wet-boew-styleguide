---
published: true
layout: default-theme-wet-boew-en
title: Alignment
hide_breadcrumb: false
date_modified: 2019-04-11
---
{::nomarkdown}
{% raw %}
  <span class="wb-prettify all-pre"></span>
  <div class="row">
    <nav role="navigation" class="col-md-8">
      <div class="panel panel-default">
        <header class="panel-heading">
          <h2 class="panel-title">Table of contents</h2>
        </header>
        <div class="panel-body">
          <ul>
            <li><a href="#purpose">Purpose</a></li>
            <li><a href="#design">Design and coding</a>
              <ul>
                <li><a href="#basic">Basic use</a>
                  <ul>
                    <li><a href="#left">Left aligned text</a></li>
                    <li><a href="#centre">Centre aligned text</a></li>
                    <li><a href="#centre-bl">Centre content blocks</a></li>
                    <li><a href="#right">Right aligned text  </a></li>
                  </ul>
                </li>
              </ul>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <section class="col-md-4">
      <div class="panel panel-warning">
        <div class="panel-body">
          <h2 class="mrgn-tp-0 h4 text-warning"><span class="fa fa-exclamation-triangle"></span> Work in progress</h2>
          <p>This page is a work in progress.</p>
          <p>Please <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">file an issue</a> or submit a pull request if information or coding is missing, incorrect or out of sync with the main repository (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <section>
    <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Purpose</h2>
    <p>Use  to align text to  the left, centre or right. Or, use to align a block of content or an image to  the centre.</p>
  </section>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="left"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-left fa-stack-1x fa-inverse"></span></span> Left aligned text</h4>
  <p>Use to align text to the left.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-left">(Content goes here)</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Apply <code>.text-left</code> to an element to left align the text within it</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use to align non-text information</li>
      </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p <strong>class=&quot;text-left&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="centre"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-center fa-stack-1x fa-inverse"></span></span> Centre aligned text</h4>
  <p>Use to align text to the centre.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-center">(Content goes here)</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Apply <code>.text-center</code> to an element to centre align the text within it</li>
		<li>Apply, if required, to table data cells to mimic accounting tables</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>

		<li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Avoid unless it adds value to the content.<br>
          <blockquote><p>Centered and right aligned text both have a “ragged” left edged which has been shown to impede reading speed and comprehension. The straight (or “hard”) left edge and ragged right edge combination of standard left aligned text performs best for  readers because it helps the eye find the start of the next line when it leaves the end of the last one.</p>
		    <footer class="text-right"><a href="https://mrwweb.com/no-justification-dont-use-right-center-and-full-justification-on-the-web/" >No Justification: Don’t Use Right, Center, and Full Justification on the Web</a></footer>
	      </blockquote>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p <strong>class=&quot;text-center&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="centre-bl"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-center fa-stack-1x fa-inverse"></span></span> Centre content blocks</h4>
  <p>Use to centre the block as a whole, including the text. Center block takes a fixed width element, and  applies an equal left and right margin, thus centering the content.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <img src="https://placehold.it/140x140" class="img-rounded center-block" alt="A generic square placeholder image with rounded corners" /> </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Apply <code>.center-block</code> to a fixed width block  element to center align it</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Avoid unless it adds value to the content.<br>
          <blockquote><p>Centered and right aligned text both have a “ragged” left edged which has been shown to impede reading speed and comprehension. The straight (or “hard”) left edge and ragged right edge combination of standard left aligned text performs best for  readers because it helps the eye find the start of the next line when it leaves the end of the last one.</p>
		    <footer class="text-right"><a href="https://mrwweb.com/no-justification-dont-use-right-center-and-full-justification-on-the-web/" >No Justification: Don’t Use Right, Center, and Full Justification on the Web</a></footer>
	      </blockquote>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;img <strong>class=&quot;center-block&quot;</strong> alt=&quot;...&quot; src=&quot;x.jpg&quot; /&gt;</code></pre>
    </div>
  </div>
  <h4 id="right"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-right fa-stack-1x fa-inverse"></span></span> Right aligned text</h4>
  <p>Use to align text to the right.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-right">(Content goes here)</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Apply <code>.text-right</code> to an element to right align the text within it</li>
		<li>Apply, if required, to table data cells to mimic accounting tables</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
       <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
       <li>Avoid unless it adds value to the content.
         <blockquote><p>Centered and right aligned text both have a “ragged” left edged which has been shown to impede reading speed and comprehension. The straight (or “hard”) left edge and ragged right edge combination of standard left aligned text performs best for  readers because it helps the eye find the start of the next line when it leaves the end of the last one.</p>
		     <footer class="text-right"><a href="https://mrwweb.com/no-justification-dont-use-right-center-and-full-justification-on-the-web/" >No Justification: Don’t Use Right, Center, and Full Justification on the Web</a></footer>
	      </blockquote>
       </li>
      </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p <strong>class=&quot;text-right&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
