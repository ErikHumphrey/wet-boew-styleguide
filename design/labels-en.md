---
published: true
layout: default-theme-wet-boew-en
title: Labels
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
                    <li><a href="#default">Default label </a></li>
                    <li><a href="#primary">Primary label</a></li>
                    <li><a href="#success">Success label</a></li>
                    <li><a href="#info">Info label</a></li>
                    <li><a href="#warning">Warning label</a></li>
                    <li><a href="#danger">Danger label</a></li>
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
  <p>Use the appropriate label to describe and highlight text-based (non-numerical) information.</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default label</h4>
  <p>Use to feature a few words within a coloured background. It provides additional context about the adjacent content. </p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Some text here <span class="label label-default">(Label info)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.label-default</code> to call attention to a section of content by adding short, text-based bits of  supporting information</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use in alerts or buttons</li>
        <li>Do not use to highlight unread items − use <a href="badges-en.html">Badges</a></li>
        <li>Do not highlight large sections of text − use <a href="alerts-en.html">Alerts</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Some text here <strong>&lt;span class=&quot;label label-default&quot;&gt;</strong>(Label info)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="primary"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-certificate fa-stack-1x fa-inverse"></span></span> Primary label</h4>
  <p>Use to feature a few words within a coloured background that matches the colour theme of the site. It provides additional context about the adjacent content.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Some text here <span class="label label-primary">(Label info)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.label-primary</code> to call attention to a section of content by adding short, text-based bits of  supporting information</li>
        <li>Use to match the label to the colour theme of the site</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use in alerts or buttons</li>
        <li>Do not use to highlight unread items − use <a href="badges-en.html">Badges</a></li>
        <li>Do not highlight large sections of text − use <a href="alerts-en.html">Alerts</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Some text here <strong>&lt;span class=&quot;label label-primary&quot;&gt;</strong>(Label info)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="success"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-check fa-stack-1x fa-inverse"></span></span> Success label</h4>
  <p>Use to feature a few words within a coloured background to suggest the content is correct. It provides additional context about the adjacent content.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-success">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Some text here <span class="label label-success">(Label info)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.label-success</code> to call attention to a section of content by adding short, text-based bits of  supporting information</li>
        <li>Use to indicate that the content is correct</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use in alerts or buttons</li>
        <li>Do not use to highlight unread items − use <a href="badges-en.html">Badges</a></li>
        <li>Do not highlight large sections of text − use <a href="alerts-en.html">Alerts</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Some text here <strong>&lt;span class=&quot;label label-success&quot;&gt;</strong>(Label info)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="info"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Info label</h4>
  <p>Use to feature a few words within a coloured background to suggest the content is informative. It provides additional context about the adjacent content.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Some text here <span class="label label-info">(Label info)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.label-info</code> to call attention to a section of content by adding short, text-based bits of  supporting information</li>
        <li>Use to indicate that the content is informative in nature</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use in alerts or buttons</li>
        <li>Do not use to highlight unread items − use <a href="badges-en.html">Badges</a></li>
        <li>Do not highlight large sections of text − use <a href="alerts-en.html">Alerts</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Some text here <strong>&lt;span class=&quot;label label-info&quot;&gt;</strong>(Label info)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="warning"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-triangle fa-stack-1x fa-inverse"></span></span> Warning label</h4>
  <p>Use to feature a few words within a coloured background to suggest that the user needs to be warned. It provides additional context about the adjacent content.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Some text here <span class="label label-warning">(Label info)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.label-warning</code> to call attention to a section of content by adding short, text-based bits of  supporting information</li>
        <li>Use to indicate that the user needs to be warned</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use in alerts or buttons</li>
        <li>Do not use to highlight unread items − use <a href="badges-en.html">Badges</a></li>
        <li>Do not highlight large sections of text − use <a href="alerts-en.html">Alerts</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Some text here <strong>&lt;span class=&quot;label label-warning&quot;&gt;</strong>(Label info)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="danger"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-circle fa-stack-1x fa-inverse"></span></span> Danger label</h4>
  <p>Use to feature a few words within a coloured background to suggest that the content  or action is dangerous. It provides additional context about the adjacent content.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Some text here <span class="label label-danger">(Label info)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.label-danger</code> to call attention to a section of content by adding short, text-based bits of  supporting information</li>
        <li>Use to indicate that the content or action is dangerous</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use in alerts or buttons</li>
        <li>Do not use to highlight unread items − use <a href="badges-en.html">Badges</a></li>
        <li>Do not highlight large sections of text − use <a href="alerts-en.html">Alerts</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Some text here <strong>&lt;span class=&quot;label label-danger&quot;&gt;</strong>(Label info)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
