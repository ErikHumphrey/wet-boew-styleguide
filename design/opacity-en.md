---
published: true
layout: default-theme-wet-boew-en
title: Opacity
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
  <p>Use to adjust the opacity of any element. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>
  <p>Use to apply an opacity/transparency to a foreground item so the background becomes visible.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Default:</p>
          <div class="row mrgn-bttm-md">
            <div class="col-sm-4"><img class="img-responsive" src="https://placehold.it/140x140" alt="Default image, a grey aquare"></div>
          </div>
          <p>With opacity:</p>
          <div class="row">
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-100</code></p><img class="opct-100 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-100"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-90</code></p><img class="opct-90 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-90"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-80</code></p><img class="opct-80 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-80"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-70</code></p>
              <img class="opct-70 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-70"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-60</code></p><img class="opct-60 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-60"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-50</code></p><img class="opct-50 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-50"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-40</code></p><img class="opct-40 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-40"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-30</code></p><img class="opct-30 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-30"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-20</code></p><img class="opct-20 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-20"></div>
            <div class="col-sm-4"><p class="mrgn-bttm-sm"><code>opct-10</code></p><img class="opct-10 img-responsive mrgn-bttm-md" src="https://placehold.it/140x140" alt="Demo of opct-10"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.opct-90</code> to <code>.opct-10</code> change the opacity of a foreground element, and make  the background visible through it        <ul>
            <li>The opacity levels vary by degrees of 10</li>
            <li>The style <code>.opct-100</code> gives an image full visibility, much like the default setting</li>
            <li>The style <code>.opct-10</code> gives an image 10% visibility</li>
          </ul>
        </li>
        <li>Use <code>.opct-100</code> when a fade in to 100%, or fade out from 100% is required</li>
        <li> Ensure that the new lighter text colour still passes accessibility colour contrast requirements        <ul>
            <li>The <a href="https://webaim.org/resources/contrastchecker/" rel="external">Color Contrast Checker <span  class="wb-inv"> (external link)</span></a> validates colours for compliance</li>
            <li>The opacity affects the whole element and everything within it</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use if the opacity makes the foreground content difficult to see or read</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre>&lt;img <strong>class=&quot;opct-100&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-90&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-80&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-70&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-60&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-50&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-40&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-30&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-20&quot;</strong> src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;
&lt;img <strong>class=&quot;opct-10&quot; </strong>src=&quot;x.jpg&quot; alt=&quot;&quot;&gt;</pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="position-en.html">Absolute positioning</a></li>
  </ul>
{% endraw %}
{:/}
