---
published: true
layout: default-theme-wet-boew-en
title: Colour
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
                    <li><a href="#addon">Add-on features</a> </li>
                  </ul>
                </li>
              </ul>
            </li>
			<li><a href="#supporting">Supporting principles</a></li>
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
  <p>Use  colour as a presentation element for either decorative purposes or to convey  information. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="muted"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-adjust fa-stack-1x fa-inverse"></span></span> Muted</h4>
  <p>Use to make text appear  gray (muted) in colour.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-muted">This text is styled with <code>.text-muted</code>.</p>
          <p>Coloured icon: <span class="fa fa-adjust text-muted"></span></p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to  de-emphasize  text (make less obvious)</li>
        <li>Wrap text in a <code>&lt;span&gt;</code> tag if a style does not appear as it is meant to, due to specificity reasons</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use as the only way to communicate information or intent, as colour alone is not accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Muted text:
&lt;p <strong>class=&quot;text-muted&quot;</strong>&gt;...&lt;/p&gt;

//  Muted icon:
&lt;span class=&quot;fa fa-adjust <strong>text-muted</strong>&quot;&gt;&lt;/span&gt;</code></pre>
    </div>
  </div>
  <h4 id="primary"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-tint fa-stack-1x fa-inverse"></span></span> Primary colour</h4>
  <p>Use to style primary information. The options include medium blue text, an icon of a blue drip, or white text with a medium blue background. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-primary">This text is styled with <code>.text-primary</code>.</p>
          <p>Coloured icon: <span class="fa fa-tint text-primary"></span></p>
          <p class="bg-primary">This text is styled with <code>.bg-primary</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to match text to the main colour palette of the site</li>
        <li> Wrap text in a <code>&lt;span&gt;</code> tag if a style does not appear as it is meant to,  due to specificity reasons</li>
        <li>Be aware that blue text can cause usability problems, as it can be mistaken for a link</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
<li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
<li>Do not use as the only way to communicate information or intent, as colour alone is not accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Primary text:
&lt;p <strong>class=&quot;text-primary&quot;</strong>&gt;...&lt;/p&gt;

// Primary icon:
&lt;span class=&quot;fa fa-tint<strong> text-primary</strong>&quot;&gt;&lt;/span&gt;

// Primary background:
&lt;p <strong>class=&quot;bg-primary&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="success"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-check fa-stack-1x fa-inverse"></span></span> Success colour</h4>
  <p>Use to style success information. This style includes options for green text, an icon of a green check mark, or default text with a pale green background. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-success">This text is styled with <code>.text-success</code>.</p>
          <p>Coloured icon: <span class="fa fa-check text-success"></span></p>
          <p class="bg-success">This text is styled with <code>.bg-success</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to suggest that the content is correct or the right way of doing something</li>
        <li> Wrap text in a <code>&lt;span&gt;</code> tag if a style does not appear as it is meant to due to specificity reasons</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>

        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use as the only way to communicate information or intent, as colour alone is not accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Success text:
&lt;p <strong>class=&quot;text-success&quot;</strong>&gt;...&lt;/p&gt;

// Success icon:
&lt;span class=&quot;fa fa-check <strong>text-success</strong>&quot;&gt;&lt;/span&gt;

// Success background:
&lt;p <strong>class=&quot;bg-success&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="info"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Info colour</h4>
  <p>Use to style fairly important information. This style includes options for blue text, an icon of a blue &quot;i&quot;, or default text with a pale blue background. </p>

  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-info">This text is styled with <code>.text-info</code>.</p>
          <p>Coloured icon: <span class="fa fa-info text-info"></span></p>
          <p class="bg-info">This text is styled with <code>.bg-info</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to highlight fairly important information</li>
        <li> Wrap text in a <code>&lt;span&gt;</code> tag if a style does not appear as it is meant to due to specificity reasons</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
<li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
<li>Do not use as the only way to communicate information or intent, as colour alone is not accessible</li>
</ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Info text:
&lt;p <strong>class=&quot;text-info&quot;</strong>&gt;...&lt;/p&gt;

// Info icon:
&lt;span class=&quot;fa fa-info <strong>text-info</strong>&quot;&gt;&lt;/span&gt;

// Info background:
&lt;p <strong>class=&quot;bg-info&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="warning"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-triangle fa-stack-1x fa-inverse"></span></span> Warning colour</h4>
  <p>Use to style warning information. This style includes options for brown text, an icon of a brown exclamation mark in a triangle, or default text with a pale golden-brown background. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-warning">This text is styled with <code>.text-warning</code>.</p>
          <p>Coloured icon: <span class="fa fa-exclamation-triangle text-warning"></span></p>
          <p class="bg-warning">This text is styled with <code>.bg-warning</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to call attention to the content and warn the user of something</li>
        <li> Wrap text in a <code>&lt;span&gt;</code> tag if a style does not appear as it is meant to due to specificity reasons</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
<li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
<li>Do not use as the only way to communicate information or intent, as colour alone is not accessible</li>
</ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Warning text:
&lt;p <strong>class=&quot;text-warning&quot;</strong>&gt;...&lt;/p&gt;

// Warning icon:
&lt;span class=&quot;fa fa-exclamation-triangle <strong>text-warning</strong>&quot;&gt;&lt;/span&gt;

// Warning background:
&lt;p <strong>class=&quot;bg-warning&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="danger"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-circle fa-stack-1x fa-inverse"></span></span> Danger colour</h4>
  <p>Use to style very important information. This style includes options for red text, an icon of a  red exclamation mark in a circle, or default text with a pale red background. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-danger">This text is styled with <code>.text-danger</code>.</p>
          <p>Coloured icon: <span class="fa fa-exclamation-circle text-danger"></span></p>
          <p class="bg-danger">This text is styled with <code>.bg-danger</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to call attention to very important content, and advise the user that an action is dangerous</li>
        <li> Wrap text in a <code>&lt;span&gt;</code> tag if a style does not appear as it is meant to due to specificity reasons</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>

        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use as the only way to communicate information or intent, as colour alone is not accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Danger text:
&lt;p <strong>class=&quot;text-danger&quot;</strong>&gt;...&lt;/p&gt;


// Danger icon:
&lt;span class=&quot;fa fa-exclamation-circle <strong>text-danger</strong>&quot;&gt;&lt;/span&gt;

// Danger background:
&lt;p <strong>class=&quot;bg-danger&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="icons-en.html">Icons</a></li>
  </ul>

   <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Supporting principles</h2>
  <div data-ajax-replace="../writing/strctr-en.html #colour-info"></div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
