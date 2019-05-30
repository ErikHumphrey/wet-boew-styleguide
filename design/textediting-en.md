---
published: true
layout: default-theme-wet-boew-en
title: Text editing effects
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
            <li> <a href="#design">Design and coding</a>
              <ul>
                <li> <a href="#basic">Basic use</a>
                  <ul>
                    <li><a href="#marked">Marked text</a></li>
                    <li> <a href="#deleted">Deleted text</a> </li>
                    <li><a href="#strikethrough">Strikethrough text</a></li>
                    <li><a href="#inserted">Inserted text</a></li>
                    <li><a href="#underlined">Underlined text</a></li>
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
  <p>Use to indicate text edits on a page.</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="marked"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-edit fa-stack-1x fa-inverse"></span></span> Marked text</h4>
  <p>Use to highlight a section of text for reference purposes, due to its relevance in another context.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Regular text plus
            <mark>marked text</mark>
            .</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use to mark information that <strong>is important in another context</strong></li>
        <li>Highlight text to show matching search terms or to show text in  relation to something else</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use in place of bold (<code>&lt;strong&gt;</code>) text
          <ul>
            <li>This tag is <strong>not meant </strong>to simply highlight  key words, phrases, numbers or amount totals</li>
          </ul>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;mark&gt;...&lt;/mark&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="deleted"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-trash-alt fa-stack-1x fa-inverse"></span></span> Deleted text</h4>
  <p>Use to indicate text was deleted.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Regular text plus <del>deleted text</del>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use to show <strong>recently deleted text</strong></li>
        <li>Use sparingly, as it makes a page difficult to read</li>
        <li>Use to show record changes to an official document, such as meeting minutes or a law</li>
        <li>Use as a temporary effect on a page </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;del&gt;...&lt;/del&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="strikethrough"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-strikethrough fa-stack-1x fa-inverse"></span></span> Strikethrough text</h4>
  <p>Use to indicate text that is no longer relevant.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Regular text plus <s>strikethrough text</s>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use to show something is <strong>no longer accurate </strong>or<strong> no longer relevant</strong></li>
        <li>Use sparingly, as it makes a page difficult to read</li>
        <li>Use to show record changes to an official document, such as meeting minutes or a law</li>
        <li>Use as a temporary effect on a page </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;s&gt;...&lt;/s&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="inserted"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-plus fa-stack-1x fa-inverse"></span></span> Inserted text</h4>
  <p>Use to indicate additions to a document. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Regular text plus <ins>inserted text</ins>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li><strong>Do not use this feature </strong>
          <ul>
            <li>It  mimics the visual appearance of a link, which  causes usability problems</li>
            <li>Non-links <strong>should not </strong>look like links </li>
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
      <pre><code>&lt;p&gt;...<strong>&lt;ins&gt;...&lt;/ins&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="underlined"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-underline fa-stack-1x fa-inverse"></span></span> Underlined text</h4>
  <p>Use to underline text. Do not use this feature on  webpages.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Regular text plus <u>underlined text</u>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li><strong>Do not use this feature </strong>
<ul>
            <li>It  mimics the visual appearance of a link, which  causes usability problems</li>
            <li>Non-links <strong>should not </strong>look like links</li>
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
      <pre><code>&lt;p&gt;...<strong>&lt;u&gt;...&lt;/u&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
