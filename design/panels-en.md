---
published: true
layout: default-theme-wet-boew-en
title: Panels
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
  <p>Use to create a visual grouping of content. Panels have colour themed options, as well as offer a distinct header and footer. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="stacking"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-list-alt fa-stack-1x fa-inverse"></span></span> Stacking options</h4>
  <p>Use to create  various container types. A panel can be broken up into a <code>.panel</code>,
    <code>.panel-heading</code>, <code>.panel-title</code>, <code>panel-body</code> and <code>.panel-footer</code>. Only the <code>.panel</code> is required. All the rest are optional.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <h6>Padded content:</h6>
          <div class="panel panel-default">
            <div class="panel-body">
              <p>Content</p>
            </div>
          </div>
          <h6>Full-width content:</h6>
          <div class="panel panel-default">
            <table class="table">
            <caption class="wb-inv">Caption text</caption>
              <thead>
                <tr>
                  <th>Table header</th>
                  <th>Table header</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Table data</td>
                  <td>Table data</td>
                </tr>
                <tr>
                  <td>Table data</td>
                  <td>Table data</td>
                </tr>
              </tbody>
            </table>
          </div>
          <h6>Padded plus full-width content:</h6>
          <div class="panel panel-default">
            <div class="panel-body">
              <p>Content</p>
            </div>
            <table class="table">
            <caption class="wb-inv">
            Caption  text</caption>
              <thead>
                <tr>
                  <th>Table header</th>
                  <th>Table header</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Table data</td>
                  <td>Table data</td>
                </tr>
                <tr>
                  <td>Table data</td>
                  <td>Table data</td>
                </tr>
              </tbody>
            </table>
          </div>
          <h6>Add a heading and/or footer:</h6>
          <div class="panel panel-default">
            <header class="panel-heading">
              <h5 class="panel-title">Panel title</h5>
            </header>
            <div class="panel-body">
              <p>Content</p>
            </div>
            <footer class="panel-footer">Panel footer</footer>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use to call attention to a specific segment of noteworthy content        <ul>
            <li><strong>Required <abbr title="cascading style sheet">CSS</abbr>: </strong><code>.panel</code></li>
            <li><strong>Optional <abbr title="cascading style sheet">CSS</abbr>: </strong><code>.panel-heading</code>, <code>.panel-title</code>, <code>.panel-body</code> and <code>.panel-footer</code></li>
          </ul>
        </li>
        <li>Ensure a heading <code>&lt;h*&gt;</code> is used within the <code>.panel-heading</code></li>
		<li>Use <code>.panel</code> for both full-width content, as well as content that is padded in from the border with <code>.panel-body</code></li>
		<li>Include a <code>&lt;caption&gt;</code> when the <code>&lt;table&gt;</code> is not directly under an <code>&lt;h*&gt;</code> tag</li>
		<li>Use <code>.wb-inv</code>
when it is necessary to make the caption invisible
               <ul>
                <li>This ensures accessibility</li>
              </ul>
		  </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span>.<br>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>//Padded content:
&lt;div <strong>class=&quot;panel panel-default&quot;</strong>&gt;
  &lt;div <strong>class=&quot;panel-body&quot;</strong>&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
&lt;/div&gt;

//Full-width content, invisible caption:
&lt;div <strong>class=&quot;panel panel-default&quot;</strong>&gt;
  <strong>&lt;table class=&quot;table&quot;&gt;</strong>
  <strong>&lt;caption class=&quot;wb-inv&quot;&gt;</strong>Caption text&lt;/caption&gt;
   ...
  &lt;/table&gt;
&lt;/div&gt;

//Padded plus full-width content:
<strong>&lt;div class=&quot;panel panel-default&quot;&gt;
  &lt;div class=&quot;panel-body&quot;&gt;</strong>
   <strong>&lt;p&gt;</strong>...&lt;/p&gt;
  &lt;/div&gt;
  <strong>&lt;table class=&quot;table&quot;&gt;</strong>
   ...
  &lt;/table&gt;
&lt;/div&gt;

//Add a heading and/or footer:
&lt;div class=&quot;panel panel-default&quot;&gt;
  <strong>&lt;header class=&quot;panel-heading&quot;&gt;</strong>
   &lt;h5 <strong>class=&quot;panel-title&quot;</strong>&gt;...&lt;/h5&gt;
  &lt;/header&gt;
  &lt;div class=&quot;panel-body&quot;&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
  &lt;footer <strong>class=&quot;panel-footer&quot;</strong>&gt;...&lt;/footer&gt;
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default panel</h4>
  <p>Use to spotlight general information/actions within a self-contained box.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <section class="panel panel-default mrgn-bttm-0">
            <header class="panel-heading">
              <h5 class="panel-title">Panel title </h5>
            </header>
            <div class="panel-body">
              <p>Panel content</p>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>

        <li>Use <code>.panel-heading</code>, <code>.panel-title</code> and  <code>.panel-body</code> to spotlight general information/actions within a self-contained box</li>
        <li>Ensure all compliance points are adhered to in <a href="#stacking">stacking options</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span>.<br>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;section<strong> class=&quot;panel panel-default&quot;</strong>&gt;
  &lt;header <strong>class=&quot;panel-heading&quot;</strong>&gt;
   &lt;h5 <strong>class=&quot;panel-title&quot;</strong>&gt;...&lt;/h5&gt;
  &lt;/header&gt;
  &lt;div <strong>class=&quot;panel-body&quot;</strong>&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
&lt;/section&gt;</code></pre>
    </div>
  </div>




  <h4 id="primary"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-tint fa-stack-1x fa-inverse"></span></span> Primary panel</h4>
  <p>Use to spotlight general information/actions within a self-contained box.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <section class="panel panel-primary mrgn-bttm-0">
            <header class="panel-heading">
              <h5 class="panel-title">Panel title </h5>
            </header>
            <div class="panel-body">
              <p>Panel content</p>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use <code>.panel-primary</code> to spotlight general information/actions within a self-contained box</li>
        <li>Ensure all compliance points are adhered to in <a href="#stacking">stacking options</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span>.<br>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;section <strong>class=&quot;panel panel-primary&quot;</strong>&gt;
  &lt;header class=&quot;panel-heading&quot;&gt;
   &lt;h5 class=&quot;panel-title&quot;&gt;...&lt;/h5&gt;
  &lt;/header&gt;
  &lt;div class=&quot;panel-body&quot;&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
&lt;/section&gt;</code></pre>
    </div>
  </div>



   <h4 id="success"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-check fa-stack-1x fa-inverse"></span></span> Success panel</h4>
  <p>Use to spotlight correct information/actions within a self-contained box.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <section class="panel panel-success mrgn-bttm-0">
            <header class="panel-heading">
              <h5 class="panel-title">Panel title </h5>
            </header>
            <div class="panel-body">
              <p>Panel content</p>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
        <li>Use <code>.panel-success</code> to spotlight correct information/actions within a self-contained box</li>
        <li>Ensure all compliance points are adhered to in <a href="#stacking">stacking options</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span>.<br>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;section <strong>class=&quot;panel panel-success&quot;</strong>&gt;
  &lt;header class=&quot;panel-heading&quot;&gt;
   &lt;h5 class=&quot;panel-title&quot;&gt;...&lt;/h5&gt;
  &lt;/header&gt;
  &lt;div class=&quot;panel-body&quot;&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
&lt;/section&gt;</code></pre>
    </div>
  </div>



   <h4 id="info"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Info panel</h4>
  <p>Use to spotlight specialized information/actions within a self-contained box..</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <section class="panel panel-info mrgn-bttm-0">
            <header class="panel-heading">
              <h5 class="panel-title">Panel title </h5>
            </header>
            <div class="panel-body">
              <p>Panel content</p>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>

        <li>Use <code>.panel-info</code> to spotlight specialized information/actions within a self-contained box</li>
        <li>Ensure all compliance points are adhered to in <a href="#stacking">stacking options</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span>.<br>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;section <strong>class=&quot;panel panel-info&quot;</strong>&gt;
  &lt;header class=&quot;panel-heading&quot;&gt;
   &lt;h5 class=&quot;panel-title&quot;&gt;...&lt;/h5&gt;
  &lt;/header&gt;
  &lt;div class=&quot;panel-body&quot;&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
&lt;/section&gt;</code></pre>
    </div>
  </div>


   <h4 id="warning"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-triangle fa-stack-1x fa-inverse"></span></span> Warning panel</h4>
  <p>Use to spotlight warning information/actions within a self-contained box.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <section class="panel panel-warning mrgn-bttm-0">
            <header class="panel-heading">
              <h5 class="panel-title">Panel title </h5>
            </header>
            <div class="panel-body">
              <p>Panel content</p>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>

        <li>Use <code>.panel-warning</code> to spotlight warning information/actions within a self-contained box</li>
        <li>Ensure all compliance points are adhered to in <a href="#stacking">stacking options</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span>.<br>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;section <strong>class=&quot;panel panel-warning&quot;</strong>&gt;
  &lt;header class=&quot;panel-heading&quot;&gt;
   &lt;h5 class=&quot;panel-title&quot;&gt;...&lt;/h5&gt;
  &lt;/header&gt;
  &lt;div class=&quot;panel-body&quot;&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
&lt;/section&gt;</code></pre>
    </div>
  </div>



   <h4 id="danger"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-circle fa-stack-1x fa-inverse"></span></span> Danger panel</h4>
  <p>Use to spotlight dangerous  information/actions within a self-contained box.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <section class="panel panel-danger mrgn-bttm-0">
            <header class="panel-heading">
              <h5 class="panel-title">Panel title </h5>
            </header>
            <div class="panel-body">
              <p>Panel content</p>
            </div>
          </section>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
<li>Use <code>.panel-danger</code> to spotlight dangerous  information/actions within a self-contained box</li>
<li>Ensure all compliance points are adhered to in <a href="#stacking">stacking options</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul><li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span>.<br>
      </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;section <strong>class=&quot;panel panel-danger&quot;</strong>&gt;
  &lt;header class=&quot;panel-heading&quot;&gt;
   &lt;h5 class=&quot;panel-title&quot;&gt;...&lt;/h5&gt;
  &lt;/header&gt;
  &lt;div class=&quot;panel-body&quot;&gt;
   &lt;p&gt;...&lt;/p&gt;
  &lt;/div&gt;
&lt;/section&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/equalheight/equalheight-en.html"  class="btn btn-default">Equalize (Equal height)</a></li>
    <li><a href="proximity-en.html" class="btn btn-default">Margin proximity </a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
