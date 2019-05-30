---
published: true
layout: default-theme-wet-boew-en
title: Keyboard keys
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
                <li><a href="#basic">Basic use</a></li>
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
    <p>Use  to mimic the keys of a computer keyboard. </p>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
    <h3 id="basic">Basic use</h3>
	 <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>

    <p>Use to present keyboard keys.</p>
    <div class="row">
      <div class="col-md-4">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
            <p>Press <kbd>Shift</kbd></p>
            <p>Press <kbd><abbr title="Control">Ctrl</abbr></kbd></p>
            <p>Press <kbd>Enter</kbd></p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
          <li>Use  <code>&lt;kbd&gt;</code> to describe a keyboard key that a user is to select in a process</li>
              <li>Use the exact spelling, spacing and sentence case of the keyboard text (for example, <kbd>Ctrl</kbd>)</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
          <li>Do not use for menu names, or content text</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;p&gt;Press <strong>&lt;kbd&gt;</strong>Shift<strong>&lt;/kbd&gt;</strong>&lt;/p&gt;
&lt;p&gt;Press &lt;kbd&gt;&lt;abbr title=&quot;Control&quot;&gt;Ctrl&lt;/abbr&gt;&lt;/kbd&gt;&lt;/p&gt;
&lt;p&gt;Press &lt;kbd&gt;Enter&lt;/kbd&gt;&lt;/p&gt;</code></pre>
      </div>
    </div>
  </section>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
