---
published: true
layout: default-theme-wet-boew-en
title: Links
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
  <section>
    <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Purpose</h2>
    <p>Use a link  (text and/or image) to take a user to another webpage, jump to another  location within the same webpage, or perform a user-control function determined  by client-side scripting (JavaScript). </p>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
    <h3 id="basic">Basic use</h3>
    <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>
    <p>Use a word, phrase, or image that allows the user to to interact with the content on a screen.  This can take the form of navigation, querying or content interaction.</p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0 h5">Appearance</h5>
            <p><a href="#">Default link</a></p>
            <p class="mrgn-bttm-0"><a href="#">Link and linked image.<img class="img-thumbnail left-block" alt="A generic square placeholder image with a white border around it" src="https://placehold.it/100x100"></a></p>
          </div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Use to link from one page to another</li>
          <li>Use to link from to a section on a page</li>
          <li>Use to open an <a href="https://wet-boew.github.io/wet-boew/demos/overlay/overlay-en.html" >overlay</a> or <a href="https://wet-boew.github.io/wet-boew/demos/lightbox/lightbox-en.html" >modal/lightbox</a></li>
          <li>Use to initiate an event/query </li>
          <li>Use to <span data-hveid="70">open a new outgoing email message</span></li>
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
        <pre><code>// Default link:
<strong>&lt;a href=&quot;#&quot;&gt;</strong>...&lt;/a&gt;

// Link and linked image:
<strong>&lt;a href=&quot;#&quot;&gt;&lt;img src=&quot;#&quot;</strong> alt=&quot;&quot; /&gt;&lt;/a&gt;</code></pre>
      </div>
    </div>
  </section>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a href="buttons-en.html" class="btn btn-default">Buttons</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-en.html"  class="btn btn-default">Carousel</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/details/details-en.html"   class="btn btn-default">Expand and hide (Details/summary) </a></li>
    <li><a href="listgroup-en.html" class="btn btn-default">List group</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/lightbox/lightbox-en.html"  class="btn btn-default">Modal popup (Lightbox)</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/overlay/overlay-en.html"  class="btn btn-default">Overlay </a></li>
    <li><a href="pagination-en.html" class="btn btn-default">Pagination</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-en.html"  class="btn btn-default">Tabs</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/toggle/toggle-en.html" class="btn btn-default">Toggle</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/lightbox/lightbox-en.html"  class="btn btn-default">Thumbnail and photo gallery (Lightbox) </a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Supporting principles</h2>
  <h3><span data-ajax-replace="../writing/strctr-en.html #links-heading"></span></h3>
  <div data-ajax-replace="../writing/strctr-en.html #links-info"></div>
  <h3><span data-ajax-replace="../writing/stl-en.html #scent-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-en.html #scent-info"></div>
  <h3><span data-ajax-replace="../writing/stl-en.html #parallel-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-en.html #parallel-info"></div>
  <h3><span data-ajax-replace="../writing/stl-en.html #scan-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-en.html #scan-info"></div>
  <h3><span data-ajax-replace="../writing/rchtctr-en.html #alphabetization-heading"></span></h3>
  <div data-ajax-replace="../writing/rchtctr-en.html #alphabetization-info"></div>
  <p class="mrgn-tp-lg text-muted">Note: Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
