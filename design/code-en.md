---
published: true
layout: default-theme-wet-boew-en
title: Code
hide_breadcrumb: false
date_modified: 2019-04-11
---
{::nomarkdown}
{% raw %}
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
                    <li><a href="#inline">Inline code </a></li>
                    <li><a href="#block">Code block </a></li>
                  </ul>
                </li>
                <li><a href="#enhanced">Enhanced use</a>
                  <ul>
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
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Purpose</h2>
  <p>Use  to emulate source code and display it in monospace  font. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="inline"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-code fa-stack-1x fa-inverse"></span></span> Inline code</h4>
  <p>Use to  emulate snippets of code (such as <abbr title="Hypertext Markup Language">HTML</abbr>) within a regular sentence.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Content here <code>&lt;a href=&quot;#&quot;&gt;link&lt;/a&gt;</code> content here</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Wrap snippets (one line or less) of code within a <code>&lt;code&gt;</code> tag</li>
        <li>Ensure to use <abbr title="American Standard Code for Information Interchange">ASCII</abbr> code so the code example renders properly:
          <ul>
            <li> Opening brackets (<code>&lt;</code>) = <code>&amp;lt;</code></li>
            <li>Closing brackets(<code>&gt;</code>) = <code>&amp;gt;</code></li>
            <li>Opening quote (<code>&quot;</code>) = <code>&amp;quot;</code></li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre class="wb-prettify prettyprint"><code>&lt;p&gt;... <strong>&lt;code&gt;&amp;lt;</strong>a href=<strong>&amp;quot;</strong>#<strong>&amp;quot;&amp;gt;</strong>link<strong>&amp;lt;</strong>/a<strong>&amp;gt;&lt;/code&gt;</strong> ...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="block"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-code fa-stack-1x fa-inverse"></span></span> Code block</h4>
  <p>Use to emulate multiple lines (blocks) of code (such as <abbr title="Hypertext Markup Language">HTML</abbr>).</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <pre><code><strong>&lt;pre&gt;
  &lt;code&gt;</strong>
   &lt;div class=&quot;container-fluid&quot;&gt;
    &lt;div class=&quot;row&quot;&gt;
     ...
	&lt;/div&gt;
   &lt;/div&gt;
  <strong>&lt;/code&gt;
&lt;/pre&gt;</strong></code></pre>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>&lt;pre&gt;</code> and <code>&lt;code&gt;</code> tags together to emulate a formatted  code  block</li>
        <li>Ensure to use <abbr title="American Standard Code for Information Interchange">ASCII</abbr> code so the code example renders properly:
          <ul>
            <li> Opening brackets (<code>&lt;</code>) = <code>&amp;lt;</code></li>
            <li>Closing brackets(<code>&gt;</code>) = <code>&amp;gt;</code></li>
            <li>Quote (<code>&quot;</code>) = <code>&amp;quot;</code></li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use this component within <code>&lt;span lang=fr&quot;&gt;</code> or <code>&lt;span lang=en&quot;&gt;</code>
          <ul>
            <li>Only translate non-code text</li>
          </ul>
        </li>
      </ul>
      <ul>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre class="wb-prettify prettyprint"><code><strong>&lt;pre&gt;&lt;code&gt; </strong>
&amp;lt;div class=&amp;quot;container-fluid&amp;quot;&amp;gt;
   &amp;lt;div class=&amp;quot;row&amp;quot;&amp;gt;
     ...
   &amp;lt;/div&amp;gt;
  &amp;lt;/div&amp;gt;
<strong>&lt;/code&gt;&lt;/pre&gt;</strong></code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/demos/prettify/prettify-en.html" >Code prettify</a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
