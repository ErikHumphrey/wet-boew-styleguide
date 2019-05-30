---
published: true
layout: default-theme-wet-boew-en
title: Headings
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
                    <li><a href="#secondary">Secondary text</a></li>
                    <li><a href="#underline">Underline</a></li>
                  </ul>
                </li>
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
		<p>Use  a heading to title  content  that is immediately below it. Headings are  large, bold, concise text that are hierarchical in nature.</p>
		<h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
		<h3 id="basic">Basic use</h3>
	  </section>

	  <section>
    <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>
    <p>Use headings so the search engine can properly rank your content. Headings are ranked more important than regular text. Choose headings strategically. The <code>&lt;h1&gt;</code> is the most important; the <code>&lt;h6&gt;</code> is the least important.</p>
    <div class="row">
      <div class="col-md-4">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
            <section>
              <h1>h1 heading</h1>
              <section>
                <h2>h2 heading</h2>
                <section>
                  <h3>h3 heading</h3>
                  <section>
                    <h4>h4 heading</h4>
                    <section>
                      <h5>h5 heading</h5>
                      <section>
                        <h6>h6 heading</h6>
                      </section>
                    </section>
                  </section>
                </section>
              </section>
            </section>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>

          <li>Capitalize the following:
            <ul>
              <li><strong>First</strong> word in a title </li>
              <li><strong>Proper</strong> noun (name of a person, place, title of a person or formal publication, or calendar time)</li>
              <li>First word <strong>after</strong> a colon ( <strong>:</strong> ) or endash   <code>&amp;#8211;</code> ( <strong>–</strong> ) . Use lower-case for the rest</li>
            </ul>
          </li>

          <li>Use mainly <code>&lt;h1&gt;</code> to <code>&lt;h4&gt;</code> headings to structure content        <ul>
              <li> Avoid  <code>&lt;h5&gt;</code> to   <code>&lt;h6&gt;</code> headings. Rather, consider restructuring content</li>
              <li>Ensure  information is in meaningful  content blocks (groups)</li>
            </ul>
          </li>
          <li>Place a title <strong>immediately above</strong> the content section that it relates to</li>
          <li>Understand and implement the related <a href="#supporting">supporting principles</a></li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
          <li>Do not   use headings to mimic a text size and weight</li>
          <li>Do not use for superficial styling purposes</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;h1&gt;h1 heading&lt;/h1&gt;

&lt;h2&gt;h2 heading&lt;/h2&gt;

&lt;h3&gt;h3 heading&lt;/h3&gt;

&lt;h4&gt;h4 heading&lt;/h4&gt;

&lt;h5&gt;h5 heading&lt;/h5&gt;

&lt;h6&gt;h6 heading&lt;/h6&gt;</code></pre>
      </div>
    </div>
  </section>

  <section>
    <h4 id="secondary"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class=" glyphicon glyphicon-paperclip fa-stack-1x fa-inverse"></span></span> Secondary text</h4>
    <p>Use to create lighter, secondary text in any heading.</p>
    <div class="row">
      <div class="col-md-4">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>


			<section>
              <h1>h1 heading &#8211; <span class="small">Secondary text</span></h1>
              <section>
                <h2>h2 heading &#8211; <span class="small">Secondary text</span></h2>
                <section>
                  <h3>h3 heading &#8211; <span class="small">Secondary text</span></h3>
                  <section>
                    <h4>h4 heading &#8211; <span class="small">Secondary text</span></h4>
                    <section>
                      <h5>h5 heading &#8211; <span class="small">Secondary text</span></h5>
                      <section>
                        <h6>h6 heading &#8211; <span class="small">Secondary text</span></h6>
                      </section>
                    </section>
                  </section>
                </section>
              </section>
            </section>

          </div>
        </div>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
          <li>Use the <code>.small</code> class to de-emphasize only <strong>a portion</strong> of the heading</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
          <li>Do not use  to de-emphasize primary information</li>
          <li>Do not   use headings to mimic a text size or weight</li>
          <li>Do not use for superficial styling purposes</li>
          <li>Do not use the <code>&lt;small&gt;</code> tag, as it is for defining small text (side-comments, disclaimers and "fine" print, including copyright and legal text)</li>
          </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;h1&gt;h1 heading &amp;#8211; <strong>&lt;span class=&quot;small&quot;&gt;</strong>Secondary text<strong>&lt;/span&gt;</strong>&lt;/h1&gt;

&lt;h2&gt;h2 heading &amp;#8211; &lt;span class=&quot;small&quot;&gt;Secondary text&lt;/span&gt;&lt;/h2&gt;

&lt;h3&gt;h3 heading &amp;#8211; &lt;span class=&quot;small&quot;&gt;Secondary text&lt;/span&gt;&lt;/h3&gt;

&lt;h4&gt;h4 heading &amp;#8211; &lt;span class=&quot;small&quot;&gt;Secondary text&lt;/span&gt;&lt;/h4&gt;

&lt;h5&gt;h5 heading &amp;#8211; &lt;span class=&quot;small&quot;&gt;Secondary text&lt;/span&gt;&lt;/h5&gt;

&lt;h6&gt;h6 heading &amp;#8211; &lt;span class=&quot;small&quot;&gt;Secondary text&lt;/span&gt;&lt;/h6&gt;</code></pre>
      </div>
    </div>
  </section>
  <section>
    <h4 id="underline"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-underline fa-stack-1x fa-inverse"></span></span> Underline</h4>
    <p>Use to add an underline to a heading.</p>
    <div class="row">
      <div class="col-md-4">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
            <section>
              <h1 class="page-header">h1 heading</h1>
              <section>
                <h2 class="page-header">h2 heading</h2>
                <section>
                  <h3 class="page-header">h3 heading</h3>
                  <section>
                    <h4 class="page-header">h4 heading</h4>
                    <section>
                      <h5 class="page-header">h5 heading</h5>
                      <section>
                        <h6 class="page-header">h6 heading</h6>
                      </section>
                    </section>
                  </section>
                </section>
              </section>
            </section>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
          <li>Use <code>.page-header</code> to make a heading stand out</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;h1 <strong>class=&quot;page-header&quot;</strong>&gt;h1 heading&lt;/h1&gt;

&lt;h2 class=&quot;page-header&quot;&gt;h2 heading&lt;/h2&gt;

&lt;h3 class=&quot;page-header&quot;&gt;h3 heading&lt;/h3&gt;

&lt;h4 class=&quot;page-header&quot;&gt;h4 heading&lt;/h4&gt;

&lt;h5 class=&quot;page-header&quot;&gt;h5 heading&lt;/h5&gt;

&lt;h6 class=&quot;page-header&quot;&gt;h6 heading&lt;/h6&gt;
</code></pre>
      </div>
    </div>
 </section>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="sizing-en.html">Sizing</a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Supporting principles</h2>
  <div data-ajax-replace="../writing/strctr-en.html #heading-info"></div>
  <h3><span data-ajax-replace="../writing/stl-en.html #parallel-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-en.html #parallel-info"></div>
    <h4><span data-ajax-replace="../writing/stl-en.html #gerunds-heading"></span></h4>
  <div data-ajax-replace="../writing/stl-en.html #gerunds-info"></div>
  <h3><span data-ajax-replace="../writing/rchtctr-en.html #write-heading"></span></h3>
  <div data-ajax-replace="../writing/rchtctr-en.html #write-info"></div>
  <h3><span data-ajax-replace="../writing/stl-en.html #scan-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-en.html #scan-info"></div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
