---
published: true
layout: default-theme-wet-boew-en
title: Pagination
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
                    <li> <a href="#active">Active state</a></li>
                    <li><a href="#disabled">Disabled state</a></li>
                    <li><a href="#sizing">Sizing</a></li>
                    <li><a href="#pager">Simple pager </a></li>
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
  <p>Use a  pagination index for long documents that are  best broken up over several pages. A user can select a specific page within a  document through either the &quot;Next&quot;, &quot;Previous&quot;, or (if present) the numeric pagination hyperlinks.</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>
  <p>Use to break up content and spread it over numerous pages. This makes large content sections easier to read.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <ul class="pagination">
            <li><a href="#" rel="prev">Previous</a></li>
            <li><a href="#">1 <span class="wb-inv">Go to Page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Go to Page 2</span></a></li>
            <li><a href="#" rel="next">Next</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.pagination</code> to number the separate pages of a large content section</li>
        <li>Ensure the pagination is always left-aligned</li>
        <li>Ensure the navigational links appear as a single row and <strong>don't wrap</strong>, unless   there is a valid reason to do so</li>
        <li>Add invisible text using <code>&lt;span class"wb-inv"&gt;</code> to make the links descriptive</li>
        <li>Ensure there is a space between the pagination  number and <code>&lt;span class"wb-inv"&gt;</code> to ensure screen readers correctly interpret the code</li>
        <li>Understand and implement the related <a href="#supporting">supporting principles</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;ul <strong>class=&quot;pagination&quot;</strong>&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; <strong>rel=&quot;prev&quot;</strong>&gt;Previous&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot;&gt;1 <strong>&lt;span class=&quot;wb-inv&quot;&gt;Go to Page</strong> 1&lt;/span&gt;&lt;/a&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot;&gt;2 <strong>&lt;span class=&quot;wb-inv&quot;&gt;Go to Page</strong> 2&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; <strong>rel=&quot;next&quot;</strong>&gt;Next&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="active"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-bolt fa-stack-1x fa-inverse"></span></span> Active state</h4>
  <p> Use to indicate the current page that the user is on.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <ul class="pagination">
            <li><a href="#" rel="prev">Previous</a></li>
            <li class="active"><a href="#">1 <span class="wb-inv">(current) Go to Page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Go to Page 2</span></a></li>
            <li><a href="#" rel="next">Next</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.active</code> to indicate the current page the user is on within the pagination</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;ul class=&quot;pagination&quot;&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Previous&lt;/a&gt;&lt;/li&gt;
  &lt;li <strong>class=&quot;active&quot;</strong>&gt;&lt;a href=&quot;#&quot;&gt;1 &lt;span class=&quot;wb-inv&quot;&gt;<strong>(current)</strong> Go to Page 1&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
  ...
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="disabled"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Disabled state</h4>
  <p> Use to hide unnecessary navigation for example, a &quot;Previous&quot; button if the user is on &quot;Page 1&quot; of a content section.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>&quot;Previous&quot; is disabled there therefore hidden:</p>
          <ul class="pagination">
            <li class="disabled"><a href="#" rel="prev">Previous</a></li>
            <li><a href="#">1 <span class="wb-inv">Go to Page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Go to Page 2</span></a></li>
            <li><a href="#" rel="next">Next</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li> Use <code>.disabled</code> for unclickable (hidden) links within the pagination</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;ul class=&quot;pagination&quot;&gt;
  &lt;li <strong>class=&quot;disabled&quot;</strong>&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Previous&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot;&gt;1 &lt;span class=&quot;wb-inv&quot;&gt;Go to Page 1&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
  ...
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="sizing"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-expand fa-stack-1x fa-inverse"></span></span> Sizing</h4>
  <p>Use <code>.pagination-lg</code> or <code>.pagination-sm</code> for additional pagination size options.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Default:</p>
          <ul class="pagination mrgn-tp-0 mrgn-bttm-md">
            <li><a href="#" rel="prev">Previous</a></li>
            <li><a href="#">1 <span class="wb-inv">Go to Page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Go to Page 2</span></a></li>
            <li><a href="#" rel="next">Next</a></li>
          </ul>
          <p>Large:</p>
          <ul class="pagination pagination-lg mrgn-tp-0 mrgn-bttm-md">
            <li><a href="#" rel="prev">Previous</a></li>
            <li><a href="#">1 <span class="wb-inv">Go to Page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Go to Page 2</span></a></li>
            <li><a href="#" rel="next">Next</a></li>
          </ul>
          <p>Small:</p>
          <ul class="pagination pagination-sm mrgn-tp-0 mrgn-bttm-0">
            <li><a href="#" rel="prev">Previous</a></li>
            <li><a href="#">1 <span class="wb-inv">Go to Page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Go to Page 2</span></a></li>
            <li><a href="#" rel="next">Next</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li><strong>Default sizing:</strong> Use for typical pagination</li>
        <li><strong>Small buttons:</strong> Use  when the pagination appears in  a small section of space. This reduces the button size to maximize the   amount of buttons that appear in a single row</li>
        <li><strong>Large button:</strong> Use when the pagination  needs additional  prominence on the page. Since  the default buttons already create prominence and a call to action, there is limited value/need to increasing their size</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Default:
&lt;ul class=&quot;pagination&quot;&gt;...&lt;/ul&gt;

// Large:
&lt;ul class=&quot;pagination <strong>pagination-lg</strong>&quot;&gt;...&lt;/ul&gt;

// Small:
&lt;ul class=&quot;pagination <strong>pagination-sm</strong>&quot;&gt;...&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="pager"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8644;</span></span> Simple pager</h4>
  <p>Use to create a simple pagination of just &quot;Previous&quot; and &quot;Next&quot; links.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Default</p>
          <ul class="pager">
            <li><a href="#" rel="prev">Previous</a></li>
            <li><a href="#" rel="next">Next</a></li>
          </ul>
          <p>Full justification buttons</p>
          <ul class="pager">
            <li class="previous"><a href="#" rel="prev">Previous</a></li>
            <li class="next"><a href="#" rel="next">Next</a></li>
          </ul>
          <p>Disabled state (hidden &quot;Previous&quot; button) </p>
          <ul class="pager">
            <li class="previous disabled"><a href="#" rel="prev">Previous</a></li>
            <li class="next"><a href="#" rel="next">Next</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.pager</code> when there is a need to <strong>only </strong>link to the &quot;Previous&quot; or &quot;Next&quot; page</li>
        <li>Use <code>.previous</code> and <code>.next</code> within the <code>&lt;li&gt;</code> elements to fully justify the <code>&lt;ul class=&quot;pager&quot;</code> links</li>
        <li>Understand and implement the related <a href="#supporting">supporting principles</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Default:
&lt;ul <strong>class=&quot;pager&quot;</strong>&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Previous&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; rel=&quot;next&quot;&gt;Next&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;

// Full justification buttons:
&lt;ul class=&quot;pager&quot;&gt;
  &lt;li <strong>class=&quot;previous&quot;</strong>&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Previous&lt;/a&gt;&lt;/li&gt;
  &lt;li <strong>class=&quot;next&quot;</strong>&gt;&lt;a href=&quot;#&quot; rel=&quot;next&quot;&gt;Next&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;

// Disabled state (hidden "Previous"):
&lt;ul class=&quot;pager&quot;&gt;
  &lt;li class=&quot;previous <strong>disabled</strong>&quot;&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Previous&lt;/a&gt;&lt;/li&gt;
  &lt;li class=&quot;next&quot;&gt;&lt;a href=&quot;#&quot; rel=&quot;next&quot;&gt;Next&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="buttons-en.html">Buttons</a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Supporting principles</h2>
  <h3><span data-ajax-replace="../writing/rchtctr-en.html #length-heading"></span></h3>
  <div data-ajax-replace="../writing/rchtctr-en.html #length-info"></div>
  <h3><span data-ajax-replace="../writing/stl-en.html #scent-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-en.html #scent-info"></div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
