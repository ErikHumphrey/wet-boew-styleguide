---
published: true
layout: default-theme-wet-boew-en
title: Invisible and visible content
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
                    <li><a href="#responsive">Responsive show and hide</a></li>
                    <li><a href="#invisible">Screen reader invisible content</a></li>
                    <li><a href="#general">General showing and hiding</a></li>
                    <li><a href="#print">Print showing and hiding</a></li>
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
  <p>Use  to show or hide  content − it all depends on what you need to accomplish. There are styles  specific to assistive technology (aid  screen-reader users), responsive design (view from  small to large devices), general usage (use of toggle tabs), and print (print  only necessary info).</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="responsive"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-desktop fa-stack-1x fa-inverse"></span></span> Responsive show and hide</h4>
  <p>Use to complement the presentation of content on each device. For faster mobile-friendly development, use these utility classes to show and hide content by device via media query. There are also utility classes to toggle content when it is printed.</p>
  <p>Try to use these on a limited basis, and avoid creating entirely different versions of the same site. </p>
	 <section class="alert alert-warning">
	 <h5 class="mrgn-tp-0">Limitations</h5>
	 <p>Responsive utilities are currently only available for block and table toggling. Their use with inline and table elements is currently <strong>not</strong> supported.</p>
	 </section>
  <section>
    <h5>Available classes</h5>
    <p>Use a single or combination of the available <abbr title="cascading style sheet">CSS</abbr> classes to toggle content across viewport (screen display area) breakpoints (point user needs to scroll).</p>
    <div class="table-responsive">
      <table class="table table-bordered table-striped responsive-utilities">
	  <caption>
	  Show and hide content in different viewports with <abbr title="cascading style sheet">CSS</abbr> styles
	  </caption>
        <thead>
          <tr>
            <td></td>
            <th>Extra small devices <small>Phones (&lt;768px)</small></th>
            <th>Small devices <small>Tablets (&ge;768px)</small></th>
            <th>Medium devices <small>Desktops (&ge;992px)</small></th>
            <th>Large devices <small>Desktops (&ge;1200px)</small></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th><code>.visible-xs</code></th>
            <td class="is-visible">Visible</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-hidden">Hidden</td>
          </tr>
          <tr>
            <th><code>.visible-sm</code></th>
            <td class="is-hidden">Hidden</td>
            <td class="is-visible">Visible</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-hidden">Hidden</td>
          </tr>
          <tr>
            <th><code>.visible-md</code></th>
            <td class="is-hidden">Hidden</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-visible">Visible</td>
            <td class="is-hidden">Hidden</td>
          </tr>
          <tr>
            <th><code>.visible-lg</code></th>
            <td class="is-hidden">Hidden</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-visible">Visible</td>
          </tr>
          <tr>
            <th><code>.hidden-xs</code></th>
            <td class="is-hidden">Hidden</td>
            <td class="is-visible">Visible</td>
            <td class="is-visible">Visible</td>
            <td class="is-visible">Visible</td>
          </tr>
          <tr>
            <th><code>.hidden-sm</code></th>
            <td class="is-visible">Visible</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-visible">Visible</td>
            <td class="is-visible">Visible</td>
          </tr>
          <tr>
            <th><code>.hidden-md</code></th>
            <td class="is-visible">Visible</td>
            <td class="is-visible">Visible</td>
            <td class="is-hidden">Hidden</td>
            <td class="is-visible">Visible</td>
          </tr>
          <tr>
            <th><code>.hidden-lg</code></th>
            <td class="is-visible">Visible</td>
            <td class="is-visible">Visible</td>
            <td class="is-visible">Visible</td>
            <td class="is-hidden">Hidden</td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>
  <div class="row">
    <div class="col-md-6">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Resize your browser, or load on different devices to test the responsive utility classes.</p>
          <section>
            <h4>Visible on...</h4>
            <p>Green check-marks and the text "Visible on" indicate the element <strong>is visible</strong> in your current viewport.</p>
            <div class="row responsive-utilities-test visible-on">
              <div class="col-xs-6 col-sm-3"> <span class="hidden-xs">Extra small<br />
                <code>hidden-xs</code></span> <span class="visible-xs">&#10004; Visible on x-small<br />
                <code>visible-xs</code></span> </div>
              <div class="col-xs-6 col-sm-3"> <span class="hidden-sm">Small<br />
                <code>hidden-sm</code></span> <span class="visible-sm">&#10004; Visible on small<br />
                <code>visible-sm</code></span> </div>
              <div class="clearfix visible-xs"></div>
              <div class="col-xs-6 col-sm-3"> <span class="hidden-md">Medium<br />
                <code>hidden-md</code></span> <span class="visible-md">&#10004; Visible on medium<br />
                <code>visible-md</code></span> </div>
              <div class="col-xs-6 col-sm-3"> <span class="hidden-lg">Large<br />
                <code>hidden-lg</code></span> <span class="visible-lg">&#10004; Visible on large<br />
                <code>visible-lg</code></span> </div>
            </div>
            <div class="row responsive-utilities-test visible-on">
              <div class="col-xs-6 col-sm-6"> <span class="hidden-xs hidden-sm">Extra small and small<br />
                <code>hidden-xs hidden-sm</code></span> <span class="visible-xs visible-sm">&#10004; Visible on x-small and small<br />
                <code>visible-xs visible-sm</code></span> </div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-md hidden-lg">Medium and large<br />
                <code>hidden-md hidden-lg</code></span> <span class="visible-md visible-lg">&#10004; Visible on medium and large<br />
                <code>visible-md visible-lg</code></span> </div>
              <div class="clearfix visible-xs"></div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-xs hidden-md">Extra small and medium<br />
                <code>hidden-xs hidden-md</code></span> <span class="visible-xs visible-md">&#10004; Visible on x-small and medium<br />
                <code>visible-xs visible-md</code></span> </div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-sm hidden-lg">Small and large<br />
                <code>hidden-sm hidden-lg</code></span> <span class="visible-sm visible-lg">&#10004; Visible on small and large<br />
                <code>visible-sm visible-lg</code></span> </div>
              <div class="clearfix visible-xs"></div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-xs hidden-lg">Extra small and large<br />
                <code>hidden-xs hidden-lg</code></span> <span class="visible-xs visible-lg">&#10004; Visible on x-small and large<br />
                <code>visible-xs visible-lg</code></span> </div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-sm hidden-md">Small and medium<br />
                <code>hidden-sm hidden-md</code></span> <span class="visible-sm visible-md">&#10004; Visible on small and medium<br />
                <code>visible-sm visible-md</code></span> </div>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div class="col-md-6">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p>Resize your browser, or load on different devices to test the responsive utility classes.</p>
          <section>
            <h4>Hidden on...</h4>
            <p>Green check-marks and the text "Hidden on" indicate the element <strong>is hidden</strong> in your current viewport.</p>
            <div class="row responsive-utilities-test hidden-on">
              <div class="col-xs-6 col-sm-3"> <span class="hidden-xs">Extra small<br />
                <code>hidden-xs</code></span> <span class="visible-xs">&#10004; Hidden on x-small<br />
                <code>visible-xs</code></span> </div>
              <div class="col-xs-6 col-sm-3"> <span class="hidden-sm">Small<br />
                <code>hidden-sm</code></span> <span class="visible-sm">&#10004; Hidden on small<br />
                <code>visible-sm</code></span> </div>
              <div class="clearfix visible-xs"></div>
              <div class="col-xs-6 col-sm-3"> <span class="hidden-md">Medium<br />
                <code>hidden-md</code></span> <span class="visible-md">&#10004; Hidden on medium<br />
                <code>visible-md</code></span> </div>
              <div class="col-xs-6 col-sm-3"> <span class="hidden-lg">Large<br />
                <code>hidden-lg</code></span> <span class="visible-lg">&#10004; Hidden on large<br />
                <code>visible-lg</code></span> </div>
            </div>
            <div class="row responsive-utilities-test hidden-on">
              <div class="col-xs-6 col-sm-6"> <span class="hidden-xs hidden-sm">Extra small and small<br />
                <code>hidden-xs hidden-sm</code></span> <span class="visible-xs visible-sm">&#10004; Hidden on x-small and small<br />
                <code>visible-xs visible-sm</code></span> </div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-md hidden-lg">Medium and large<br />
                <code>hidden-md hidden-lg</code></span> <span class="visible-md visible-lg">&#10004; Hidden on medium and large<br />
                <code>visible-md visible-lg</code></span> </div>
              <div class="clearfix visible-xs"></div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-xs hidden-md">Extra small and medium<br />
                <code>hidden-xs hidden-md</code></span> <span class="visible-xs visible-md">&#10004; Hidden on x-small and medium<br />
                <code>visible-xs visible-md</code></span> </div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-sm hidden-lg">Small and large<br />
                <code>hidden-sm hidden-lg</code></span> <span class="visible-sm visible-lg">&#10004; Hidden on small and large<br />
                <code>visible-sm visible-lg</code></span> </div>
              <div class="clearfix visible-xs"></div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-xs hidden-lg">Extra small and large<br />
                <code>hidden-xs hidden-lg</code></span> <span class="visible-xs visible-lg">&#10004; Hidden on x-small and large<br />
                <code>visible-xs visible-lg</code></span> </div>
              <div class="col-xs-6 col-sm-6"> <span class="hidden-sm hidden-md">Small and medium<br />
                <code>hidden-sm hidden-md</code></span> <span class="visible-sm visible-md">&#10004; Hidden on small and medium<br />
                <code>visible-sm visible-md</code></span> </div>
            </div>
          </section>
        </div>
      </div>
    </div>
  </div>
  <h4 id="invisible"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-wheelchair fa-stack-1x fa-inverse"></span></span> Screen reader invisible content</h4>
  <p>Use to clip content into a one pixel square. This creates links that are descriptive (and compliant), but don't visually clutter the page. It is common to use this technique to target assistive technology users. For example, screen-reader users hear the information, but the visual user does not hear or see it. The <abbr title="Cascading Style Sheet">CSS</abbr> attribute <code>display: none;</code> does not achieve the same effect, as screen readers ignore it entirely.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p><a class="btn btn-default" href="#">1<span class="wb-inv">: Page 1 of search results</span></a></p>
          <p>(<strong>Actual link text:</strong> 1: Page 1 of search results)</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li> Use <code>.wb-inv</code> to hide content from visual users, and to create descriptive links for assistive technology users</li>
        <li> Ensure the invisible text is concise, descriptive and unique</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;a class=&quot;button button-small&quot; href=&quot;#&quot;&gt;1<strong>&lt;span class=&quot;wb-inv&quot;&gt;</strong>: Page 1 of search results&lt;/span&gt;&lt;/a&gt;</code></pre>
    </div>
  </div>
  <h4 id="general"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-eye-slash fa-stack-1x fa-inverse"></span></span> General show and hide</h4>
  <p>Use to force an element to  show or hide with the use of <code>.show</code> or <code>.hidden</code> classes. These classes use <code>!important</code>.</p>
  <p>Use <code>.invisible</code>  to toggle <strong>only the visibility </strong>of an element; the <code>display</code> is not modified, and the element  still affects the flow of the document.</p>
  <div class="row">
    <div class="col-md-6">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use with custom JavaScript to affect the visibility of content on a page. These two classes are available for scripting solutions</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-6">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class="show"</strong>&gt;...&lt;/div&gt;
&lt;div <strong>class="hidden"</strong>&gt;...&lt;/div&gt;</code></pre>
      <pre><code>// Classes
<strong>.show</strong> {
  display: block !important;
}
<strong>.hidden</strong> {
  display: none !important;
  visibility: hidden !important;
}
<strong>.invisible</strong> {
  visibility: hidden;
}</code></pre>
    </div>
  </div>
  <h4 id="print"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-print fa-stack-1x fa-inverse"></span></span> Print show and hide</h4>

  <p>Use these  classes  to toggle content for print.</p>
  <div class="row">
    <div class="col-md-6">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use the classes <code>.visible-print</code> or <code>.hidden-print</code> to either include or exclude content when a user prints a page</li>
        <li>Prevent unnecessary content from printing, such as menus and decorative graphics</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-6">
      <div class="table-responsive">
        <table class="table table-bordered responsive-utilities">
		<caption>Show and hide content for print with <abbr title="cascading style sheet">CSS</abbr> styles</caption>
          <thead>
            <tr>
              <th>Class</th>
              <th>Browser</th>
              <th>Print</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <th><code>.visible-print</code></th>
              <td class="is-hidden">Hidden</td>
              <td class="is-visible">Visible</td>
            </tr>
            <tr>
              <th><code>.hidden-print</code></th>
              <td class="is-visible">Visible</td>
              <td class="is-hidden">Hidden</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
