---
published: true
layout: default-theme-wet-boew-en
title: Margin proximity
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
  <p>Use  to increase or decrease the proximity of one object to another. This adjusts  the white space between two elements to suggest whether items are related or  unrelated. Additionally, these classes allow grid and non-grid content to exist  in the same row. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <div class="row">
    <div class="col-sm-6 col-lg-3">
      <h4 id="top"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8613; </span></span> Margin top</h4>
      <p>Increase or decrease the default top margin of an element (heading, table, list) or design object (panel, well, grid...). </p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Details</h5>
          <ul>
            <li><code>.mrgn-tp-0</code> = 0px</li>
            <li><code>.mrgn-tp-sm</code> = 5px</li>
            <li><code>.mrgn-tp-md</code> = 15px</li>
            <li><code>.mrgn-tp-lg</code> = 30px</li>
            <li><code>.mrgn-tp-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-sm-6 col-lg-3">
      <h4 id="bottom"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8615; </span></span> Margin bottom</h4>
      <p>Increase or decrease the default bottom margin of an element (heading, table, list) or design object (panel, well, grid...). </p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Details</h5>
          <ul>
            <li><code>.mrgn-bttm-0</code> = 0px</li>
            <li><code>.mrgn-bttm-sm</code> = 5px</li>
            <li><code>.mrgn-bttm-md</code> = 15px</li>
            <li><code>.mrgn-bttm-lg</code> = 30px</li>
            <li><code>.mrgn-bttm-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
  <div class="clear visible-md"></div>
    <div class="col-sm-6 col-lg-3">
      <h4 id="left"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8612; </span></span> Margin left</h4>
      <p>Increase or decrease the default left margin of an element (heading, table, list) or design object (panel, well, grid...). </p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Details</h5>
          <ul>
            <li><code>.mrgn-lft-0</code> = 0px</li>
            <li><code>.mrgn-lft-sm</code> = 5px</li>
            <li><code>.mrgn-lft-md</code> = 15px</li>
            <li><code>.mrgn-lft-lg</code> = 30px</li>
            <li><code>.mrgn-lft-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-sm-6 col-lg-3">
      <h4 id="right"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8614; </span></span> Margin right</h4>
      <p>Increase or decrease the default right margin of an element (heading, table, list) or design object (panel, well, grid...). </p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Details</h5>
          <ul>
            <li><code>.mrgn-rght-0</code> = 0px</li>
            <li><code>.mrgn-rght-sm</code> = 5px</li>
            <li><code>.mrgn-rght-md</code> = 15px</li>
            <li><code>.mrgn-rght-lg</code> = 30px</li>
            <li><code>.mrgn-rght-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
  </div>

          <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
<p>Compliance point(s):</p>
        <ul>
            <li>Use to increase or decrease the white space in between objects</li>
			<li>Understand and implement the related  <a href="#supporting">supporting principles</a></li>
          </ul>

          <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5><p>Compliance point(s):</p><ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        </ul>

  <h3 id="enhanced">Enhanced use</h3><h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4> <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="reflow-en.html">Reflowing content around grids</a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Supporting principles</h2>
  <p>Increasing or decreasing proximity and white space suggests that content is  either associated or unrelated.</p>
  <blockquote>
    <p>The principle of proximity in visual perception is a very simple one: things that are spatially close to each other are seen as related. We can use this principle to make it clear when elements ... have an association, and when they are separate.</p>
    <p>Put things that are related close together, and space things that need to be seen as separate.</p>
    <p>We can apply the principle of proximity in reverse: elements that are spaced apart from each other are seen as separate. </p>
     <footer class="text-right">Formulate Information Design<br>
      <cite><a href="https://www.formulate.com.au/blog/perception-5-proximity" >Perception and the design of forms — Part 5: Proximity</a></cite></footer>
  </blockquote>
  <blockquote>
    <p>The principle of proximity calls for related items to be grouped visually, creating less clutter and making for a more organized layout. Items unrelated to each other should be placed further apart, to emphasize their lack of relationship.</p>
    <p>Using white space effectively and grouping related elements are critical to giving your website a clear visual hierarchy.</p>
    <footer class="text-right">Louis Lazaris<br>
      <cite><a href="https://www.webdesignerdepot.com/2010/01/the-principle-of-proximity-in-web-design/" >The Principle of Proximity in Web Design </a></cite></footer>
  </blockquote>
{% endraw %}
{:/}
