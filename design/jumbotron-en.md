---
published: true
layout: default-theme-wet-boew-en
title: Jumboton
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
                    <li><a href="#full">Full width</a></li>
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
    <p>Use  to extend the entire viewport to showcase key content on your site.</p>
  </section>
  <section>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
    <h3 id="basic">Basic use</h3>
	<h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>


    <div class="row">
      <div class="col-md-5">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>

            <section class="jumbotron">

              <p>A component for calling extra attention to featured content or information.</p>
              <p><a class="btn btn-info btn-lg" role="button" href="#">Learn more</a></p>
            </section>
          </div>
 </div>

      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Use to call attention to a specific segment of noteworthy content</li>
		  <li>Use primarily for display beyond the viewport of the container (full-screen)</li>

        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Do not use this styling if the content is confined to a <code>.container</code>, use <a href="https://wet-boew.github.io/wet-boew-styleguide/v4/design/wells-en.html">wells</a> instead </li>
		  <li>Do not use in place of more effective ways to showcase content, such as alerts, images, carousel, lead in statements, and so forth</li>
          <li>Do not use this component in a way that conflicts with the preceding compliance point(s)</li>
        </ul>
      </div>
    <div class="col-md-3">
        <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;section class=&quot;jumbotron&quot;&gt;
&lt;p&gt;...&lt;/p&gt;
&lt;p&gt;&lt;a class=&quot;btn btn-info btn-lg&quot; role=&quot;button&quot;&gt;Learn more&lt;/a&gt;&lt;/p&gt;
&lt;/section&gt;
</code></pre>
      </div>
    </div>
  <h4 id="full"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-expand fa-stack-1x fa-inverse"></span></span> Full width</h4>
<p> To make the jumbotron full width, and without rounded corners, place it outside all <code>.container</code>s. Instead add a <code>.container</code> within.</p>
  </section>
  <p class="mrgn-tp-lg">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" rel="external">Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
