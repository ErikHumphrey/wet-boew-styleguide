---
published: true
layout: default-theme-wet-boew-en
title: Badges
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
                <li><a href="#basic">Basic use</a> </li>
                <li><a href="#enhanced">Enhanced use</a>
                  <ul>
                    <li><a href="#collapsing">Self collapsing badges</a></li>
                    <li><a href="#addon">Add-on features</a> </li>
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
    <p>Use badges (numerical indicators) to highlight the number of  updates, new or unread items associated with a link.</p>
  </section>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>
  <p>Use to highlight new or updated items with a simple grey numeric, or  blue button-like badge. </p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0 h5">Appearance</h5>
          <p><a href="#">Inbox <span class="badge">42<span class="wb-inv"> unread emails</span></span></a></p>
          <p><a class="btn btn-primary" href="#">Inbox <span class="badge">42<span class="wb-inv"> unread emails</span></span></a></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Place <code>.badge</code> on the right side of the link</li>
        <li>Ensure the badge is dynamic, in that once items are actioned, the numeric value goes down</li>
        <li>Ensure it contains only numerical information</li>
        <li>Ensure the badge includes invisible text to make it descriptive.  For example: <code>&lt;p&gt;&lt;a href=&quot;#&quot;&gt;Inbox &lt;span class=&quot;badge&quot;&gt;42&lt;span class=&quot;wb-inv&quot;&gt; unread emails&lt;/span&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;</code></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger h5"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not show there are zero "0" items; if there are no items, the badge should disappear</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Grey badge:
&lt;p&gt;&lt;a href=&quot;#&quot;&gt;Inbox &lt;span <strong>class=&quot;badge&quot;</strong>&gt;42&lt;span class=&quot;wb-inv&quot;&gt; unread emails&lt;/span&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;

// Blue button-like badge:
&lt;p&gt;&lt;a <strong>class=&quot;btn btn-primary&quot;</strong> href=&quot;#&quot;&gt;Inbox &lt;span <strong>class=&quot;badge&quot;</strong>&gt;42&lt;span class=&quot;wb-inv&quot;&gt; unread emails&lt;/span&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="collapsing"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-times fa-stack-1x fa-inverse"></span></span> Self collapsing badges</h4>
  <p>Use when there are no new or unread items. Badges  simply collapse (via <abbr title="cascading style sheet">CSS</abbr> <code>:empty</code> selector). </p>
  <section class="alert alert-danger">
    <h4 class="mrgn-tp-0">Cross-browser compatibility</h4>
    <p>Badges won't self collapse in Internet Explorer 8 because it lacks support for the <code>:empty</code> selector.</p>
  </section>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p><a href="#">Inbox <span class="badge"></span></a></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Remove the content within the badge and it will self-collapse, rather than removing the badge</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// No content inside badge:
&lt;p&gt;&lt;a href=&quot;#&quot;&gt;... &lt;span <strong>class=&quot;badge&quot;</strong>&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="buttons-en.html">Buttons</a></li>
    <li><a class="btn btn-default" href="listgroup-en.html">List group</a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
