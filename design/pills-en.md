---
published: true
layout: default-theme-wet-boew-en
title: Pills
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
                    <li><a href="#default">Default</a></li>
                    <li><a href="#vertical">Vertical</a></li>
                    <li><a href="#disabled">Disabled</a></li>
                    <li><a href="#justified">Justified</a></li>
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
    <p>Use to style a navigation list and to draw focus to an active link.</p>
  </section>
  <section>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
    <h3 id="basic">Basic use</h3>
    <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>
	<p>Navigation list exists horizontally. </p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
          <ul class="nav nav-pills">
	<li class="active"><a href="#">A</a></li>
	<li><a href="#">B</a></li>
	<li><a href="#">C</a></li>
</ul></div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li><strong>Do not use this feature </strong>
            <ul>
              <li>It is inherited from Bootstrap but its intended purpose is not compatible with WET</li>
              <li>Use other options, such as <a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-en.html">Tabs</a>, <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/listgroup-en.html">List group</a> or <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/pagination-en.html">Pagination</a> for navigation purposes  </li>
            </ul>
          </li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
        <p>Compliance point(s):</p>
        <ul><li>Do not use this component in a way that conflicts with the preceding compliance point(s)</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre>&lt;ul class=&quot;nav nav-pills&quot;&gt;
 &lt;li class=&quot;active&quot;&gt;&lt;a href=&quot;#&quot;&gt;A&lt;/a&gt;&lt;/li&gt;
 &lt;li&gt;&lt;a href=&quot;#&quot;&gt;B&lt;/a&gt;&lt;/li&gt;
 &lt;li&gt;&lt;a href=&quot;#&quot;&gt;C&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;</pre>
      </div>
    </div>
    <h4 id="vertical"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-v fa-stack-1x fa-inverse"></span></span> Vertical</h4>
	<p>Navigation list exists vertically by adding <code>.nav-stacked</code>. </p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
           <ul class="nav nav-pills nav-stacked">
	<li class="active"><a href="#">A</a></li>
	<li><a href="#">B</a></li>
	<li><a href="#">C</a></li>
</ul></div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li><strong>Do not use this feature </strong>
            <ul>
              <li>It is inherited from Bootstrap but its intended purpose is not compatible with WET</li>
              <li>Use other options, such as <a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-en.html">Tabs</a>, <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/listgroup-en.html">List group</a> or <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/pagination-en.html">Pagination</a> for navigation purposes</li>
            </ul>
          </li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance point(s)</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;ul class=&quot;nav nav-pills nav-stacked&quot;&gt;
 ...
&lt;/ul&gt;</code></pre>
      </div>
    </div>
    <h4 id="disabled"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Disabled</h4>
	<p>Style a navigation list item as disabled  by adding <code>.disabled</code>.</p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
           <ul class="nav nav-pills">
	<li class="disabled"><a href="#">A</a></li>
	<li><a href="#">B</a></li>
	<li><a href="#">C</a></li>
</ul></div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
        <p>Compliance point(s):</p>
		<ul>
          <li><strong>Do not use this feature </strong>
            <ul>
              <li>It is inherited from Bootstrap but its intended purpose is not compatible with WET</li>
              <li>Use other options, such as <a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-en.html">Tabs</a>, <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/listgroup-en.html">List group</a> or <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/pagination-en.html">Pagination</a> for navigation purposes</li>
              <li>This class will only change the <code>&lt;a&gt;</code>'s appearance, not its functionality </li>
            </ul>
          </li>
	    </ul>

        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance point(s)</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;ul class=&quot;nav nav-pills&quot;&gt;
&lt;li class=&quot;disabled&quot;&gt;...&lt;/li&gt;
 ...
&lt;/ul&gt;</code></pre>
      </div>
    </div>
    <h4 id="justified"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-h fa-stack-1x fa-inverse"></span></span> Justified</h4>
	<p>Navigation list exists horizontally across entire grid column using <code>.nav-justify</code>.
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
          <ul class="nav nav-pills nav-justified">
	<li class="active"><a href="#">A</a></li>
	<li><a href="#">B</a></li>
	<li><a href="#">C</a></li>
</ul></div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
        <p>Compliance point(s):</p>
         <ul>
          <li><strong>Do not use this feature </strong>
            <ul>
              <li>It is inherited from Bootstrap but its intended purpose is not compatible with WET</li>
              <li>Use other options, such as <a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-en.html">Tabs</a>, <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/listgroup-en.html">List group</a> or <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/pagination-en.html">Pagination</a> for navigation purposes</li>
            </ul>
          </li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance point(s)</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;ul class=&quot;nav nav-pills nav-justified&quot;&gt;
 ...
&lt;/ul&gt;
</code></pre>
      </div>
    </div>
  </section>
  <p class="mrgn-tp-lg">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" rel="external">Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
