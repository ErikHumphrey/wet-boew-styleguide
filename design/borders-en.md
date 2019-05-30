---
published: true
layout: default-theme-wet-boew-en
title: Borders
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
                    <li><a href="#hr">Horizontal rule <code>&lt;hr&gt;</code></a></li>
                    <li><a href="#radius">Remove border radius</a></li>
                    <li><a href="#addon">Add-on features</a></li>
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
  <p>Use  to add single or multiple borders to design  elements in order to separate or call attention to content. Additionally,  remove default borders or sharpen corners that appear in design components such  as a &quot;well&quot;. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="left"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-270">&macr;&macr;&macr;</span></span> Left border</h4>
  <p>Use to add a left border to an element. If applied to grids, the border  appears on the outside edge of the 15px gutter.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <div class="col-md-12 brdr-lft"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use <code>.brdr-lft</code> to add a left border</li>
        <li>Use to separate or set apart content</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
     <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-lft</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="right"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-90">&macr;&macr;&macr;</span></span> Right border</h4>
  <p>Use to add a right border to an element. If applied to grids, the border  appears on the outside edge of the 15px gutter.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <div class="col-md-12 brdr-rght"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use <code>.brdr-rght</code> to add a right border</li>
        <li>Use to separate or set apart content</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-rght</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="top"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&macr;&macr;&macr;</span></span> Top border</h4>
  <p>Use to add a top border to an element. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <div class="col-md-12 brdr-tp"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use <code>.brdr-tp</code> to add a top border</li>
        <li>Use to separate or set apart content</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-tp</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="bottom"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-180">&macr;&macr;&macr;</span></span> Bottom border</h4>
  <p>Use to add a bottom border to an element.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <div class="col-md-12 brdr-bttm"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use <code>.brdr-bttm</code> to add a bottom border</li>
        <li>Use to separate or set apart content</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-bttm</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="hr"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-180">&macr;&macr;&macr;</span></span> Horizontal rule <code>&lt;hr&gt;</code></h4>
  <p>Use to apply a border to an <code>&lt;hr&gt;</code> to darken it.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Default:</p>
          <hr>
          <p>Darkened:</p>
          <hr class="brdr-bttm">
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to define a thematic change in the content, as per the correct us of an <code>&lt;hr&gt;</code></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Default:
<strong>&lt;hr&gt;</strong>

// Darkened:
&lt;hr <strong>class=&quot;brdr-bttm&quot;</strong>&gt;</code></pre>
    </div>
  </div>
  <h4 id="radius"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&lceil;</span></span> Remove border radius</h4>
  <p>Use to remove the border radius from a design component, like a <a href="wells-en.html">well</a>.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <div class="row">
            <div class="col-sm-6">
              <div class="well">
                <p>Default</p>
              </div>
            </div>
            <div class="col-sm-6">
              <div class="well brdr-rds-0">
                <p>No radius</p>
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col-sm-6">
              <div class="panel panel-default">
                <div class="panel-heading">
                  <h5 class="panel-title">Default</h5>
                </div>
                <div class="panel-body"> </div>
              </div>
            </div>
            <div class="col-sm-6">
              <div class="panel panel-default brdr-rds-0">
                <div class="panel-heading">
                  <h5 class="panel-title">No radius</h5>
                </div>
                <div class="panel-body"> </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use <code>.brdr-rds-0</code> to remove the radius of a border in a panel or a well</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// No radius in a panel:
&lt;div <strong>class=&quot;brdr-rds-0 </strong>panel panel-default&quot;&gt;
...
&lt;/div&gt;

// No radius in a well:
&lt;div <strong>class=&quot;brdr-rds-0</strong> well&quot;&gt;
...
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/equalheight/equalheight-en.html" >Equalize (Equal height)</a></li>
  </ul>
  <h2 id="supporting" tabindex="-1"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Supporting principles</h2>
  <p> The Principle of Common Region states that objects that are within the same demarcated (bordered) region are perceived as grouped together. </p>
{% endraw %}
{:/}
