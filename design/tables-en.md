---
published: true
layout: default-theme-wet-boew-en
title: Tables
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
                    <li><a href="#width">Adjust column and table widths</a></li>
                    <li><a href="#striped">Striped rows (zebra stripe)</a></li>
                    <li><a href="#hover">Hover rows</a></li>
                    <li><a href="#bordered">Bordered rows</a></li>
                    <li><a href="#condensed">Condensed rows</a></li>
                    <li><a href="#responsive">Responsive tables</a></li>
                    <!--  <li><a href="#gridify">Gridify table</a></li> -->
                    <li><a href="#colours">Coloured rows and cells </a></li>
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
  <p>Use  to organize data into rows and columns in order to create data cells. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Default</h4>
  <p>Use for  basic styling (only horizontal dividers and light padding). Add the base <code>.table</code> <abbr title="cascading style sheet">CSS</abbr> to any <code>&lt;table&gt;</code>. Given the widespread use of tables for other plugins like calendars and date pickers, this page lists some isolated custom table styles.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <h6  class="h5 mrgn-tp-xl">Heading above table</h6>
          <table class="table">
            <caption class="wb-inv">
            Table example with heading
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
            </tbody>
          </table>
          <h6  class="h5 mrgn-tp-xl">Empty cells in table </h6>
          <table class="table">
            <caption class="wb-inv">
            Table example with invisible data cells
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>-</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>-</td>
              </tr>
            </tbody>
          </table>
          <table class="table">
            <caption>
            Table caption
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use tables  to display tabular data such as financial, statistical, comparative, or numerical   information</li>
        <li>Use <code>.table</code> to style a basic table</li>
        <li>Use consistent  heading text in  related tables
          <ul>
            <li>For example, use "Name" as a header for all contact listings, not a   variety of titles such as "Contacts", "Names" or "User"</li>
          </ul>
        </li>
        <li>Insert <strong>a dash  (-) </strong> in empty data cells
          <ul>
            <li>The dash (-) allows  the  screen reader  to correctly read the content  as &quot;empty&quot;, and properly displays when magnified</li>
          </ul>
        </li>
        <li>Include the appropriate <code>scope=&quot;col&quot;</code> or <code>scope=&quot;row</code> within the <code>&lt;th&gt;</code> tag</li>
        <li>Place a  descriptive <code>&lt;h*&gt;</code> title tag <strong>directly above</strong> a table when it does not contain a <code>&lt;caption&gt;</code> tag</li>
        <li>Include a <strong>visible</strong> table caption when the <code>&lt;h*&gt;</code> title  is not directly above the table, or <strong>if multiple tables appear under </strong>an <code>&lt;h*&gt;</code> tag
          <ul>
            <li>Use a <code>&lt;caption&gt; </code> tag on all tables to ensure they  validate, and are accessible and        descriptive (especially on statistics or financial pages that contain        multiple tables)</li>
          </ul>
          <ul>
            <li>Use <code>.wb-inv</code> (as needed) to make the table caption invisible, yet ensure accessibility</li>
          </ul>
        </li>
        <li>Understand and implement the related <a href="#supporting">supporting principles</a></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use tables for layout purposes</li>
        <li>Do not use <code>title=&quot;&quot;</code> within the <code>&lt;table&gt;</code> tag</li>
        <li>Do not use <abbr title="Not Applicable">N/A</abbr>, <code>&amp;nbsp;</code> or have blank cells within a table
          <ul>
            <li>This is to avoid screen reader issues</li>
          </ul>
        </li>
        <li>Avoid merged cells, as they are complex   to code and pose accessibility issues</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Heading above table:
<strong>&lt;h*&gt;...&lt;/h*&gt;</strong>
&lt;table <strong>class="table&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Caption text&lt;/caption&gt;
  &lt;thead&gt;
   &lt;tr&gt;
     <strong>&lt;th scope=&quot;col&quot;&gt;</strong>...&lt;/th&gt;
   &lt;/tr&gt;
  &lt;/thead&gt;
  &lt;tbody&gt;
   &lt;tr&gt;
    &lt;td&gt;...&lt;/td&gt;
   &lt;tr&gt;
  &lt;/tbody&gt;
&lt;/table&gt;
</code><code>
// Empty cells in table:
&lt;table <strong>class=&quot;table&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;<strong>Caption text</strong>&lt;/caption&gt;
&lt;thead&gt;
    &lt;tr&gt;
     &lt;th scope=&quot;col&quot;&gt;...&lt;/th&gt;
     &lt;th scope=&quot;col&quot;&gt;...&lt;/th&gt;
    &lt;/tr&gt;
  &lt;/thead&gt;
  &lt;tbody&gt;
   &lt;tr&gt;
    <strong>&lt;td&gt;-&lt;/td&gt;</strong>
    <strong>&lt;td&gt;-&lt;/td&gt;</strong>
   &lt;tr&gt;
  &lt;/tbody&gt;
&lt;/table&gt;</code><code>

// Table caption:
&lt;table <strong>class=&quot;table&quot;</strong>&gt;
  <strong>&lt;caption&gt;Caption text&lt;/caption&gt;</strong>
    &lt;thead&gt;...&lt;/thead&gt;
    &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="width"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-h fa-stack-1x fa-inverse"></span></span> Adjust column and table widths</h4>
  <p>Use <a href="grids-en.html">grid <abbr title="cascading style sheet">CSS</abbr></a> to adjust the width of the columns.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <table class="table">
            <caption class="wb-inv">
            Table example with adjusted columns and width
            </caption>
            <thead>
              <tr>
                <th  scope="col"  class="col-sm-7">Header</th>
                <th  scope="col" class="col-sm-5">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Data data data</td>
                <td>Data data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Ensure the width  of the <code>&lt;table&gt;</code> as a whole, as well as each <code>&lt;th&gt;</code> column both suit the content
          <ul>
            <li>Tables with too much (over-separation) or too little (over-crowding) white space are difficult to read</li>
          </ul>
        </li>
        <li>Insert the <code>&lt;table&gt;</code> within an appropriate container to limit the overall table size</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not make all tables on a page the same width simply for design purposes</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code><strong>// </strong>table with limited column and overall width<strong>
&lt;div <strong>class=&quot;col-md-3&quot;</strong>&gt;</strong><strong>
</strong> &lt;table <strong>class=&quot;table&quot;</strong>&gt;
 &lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Caption text&lt;/caption&gt;
   &lt;thead&gt;
     &lt;tr&gt;
      &lt;th scope=&quot;col&quot; <strong>class=&quot;col-sm-8&quot;</strong>&gt;...&lt;/th&gt;
      &lt;th scope=&quot;col&quot; <strong>class=&quot;col-sm-4&quot;</strong>&gt;...&lt;/th&gt;
    &lt;/tr&gt;
   &lt;/thead&gt;
   &lt;tbody&gt;
    &lt;tr&gt;
     &lt;td&gt;...&lt;/td&gt;
     &lt;td&gt;...&lt;/td&gt;
    &lt;/tr&gt;
   &lt;/tbody&gt;
 &lt;/table&gt;
&lt;/div&gt;</code>
</pre>
    </div>
  </div>
  <h4 id="striped"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-bars fa-stack-1x fa-inverse"></span></span> Striped rows (zebra stripe) </h4>
  <p>Use to add zebra-striping to any table row.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <table class="table table-striped">
            <caption class="wb-inv">
            Table example with zebra stripes
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.table-striped</code> within the <code>&lt;tbody&gt;</code> to help  distinguish rows from each other</li>
        <li>Use mainly on long, complex tables</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>
&lt;table <strong>class=&quot;table table-striped&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Caption text&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="hover"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-hand-point-up fa-stack-1x fa-inverse"></span></span> Hover rows</h4>
  <p>Use to add a zebra-striped hover effect to any table row within the <code>&lt;tbody&gt;</code>.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <table class="table table-hover">
            <caption class="wb-inv">
            Table example with hover rows
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.table-hover</code> to allow the user to highlight each row when they mouse over it</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>
&lt;table <strong>class=&quot;table table-hover&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Caption text&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="bordered"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-table fa-stack-1x fa-inverse"></span></span> Bordered rows </h4>
  <p>Use to add borders to the table.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <table class="table table-bordered">
            <caption class="wb-inv">
            Table example with bordered rows
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.table-bordered</code> to separate information when the table cells have a lot of data in them, and word wrap
          <ul>
            <li>This makes it easy for the user to tell what information belongs to which cell</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>
&lt;table <strong>class=&quot;table table-bordered&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Caption text&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="condensed"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8615; &#8613;</span></span> Condensed rows</h4>
  <p>Use to reduce the padding within the table.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <table class="table table-condensed">
            <caption class="wb-inv">
            Table example with condensed rows
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.table-condensed</code> to narrow the row height</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>
&lt;table <strong>class=&quot;table table-condensed&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Caption text&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="responsive"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-mobile-alt fa-stack-1x fa-inverse"></span></span> Responsive tables</h4>
  <p>Create responsive tables to make a table scroll horizontally for small devices (under 768px). On anything larger than 768px wide, there is no visual difference in these tables.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <div class="table-responsive">
            <table class="table">
              <caption class="wb-inv">
              Table example with responsive design
              </caption>
              <thead>
                <tr>
                  <th scope="col">Header</th>
                  <th scope="col">Header</th>
                  <th scope="col">Header</th>
                  <th scope="col">Header</th>
                  <th scope="col">Header</th>
                  <th scope="col">Header</th>
                  <th scope="col">Header</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                </tr>
                <tr>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                </tr>
                <tr>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                  <td>Data Data</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Wrap <code>.table</code> within <code>.table-responsive</code> when the table is wide, and needs to horizontally scroll on mobile devices</li>
        <li>Split large tables into smaller ones to improve the usability of the content</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class=&quot;table-responsive&quot;</strong>&gt;
&lt;table <strong>class=&quot;table&quot;</strong>&gt;
 &lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Caption text&lt;/caption&gt;
    &lt;thead&gt;...&lt;/thead&gt;
    &lt;tbody&gt;...&lt;/tbody&gt;
  &lt;/table&gt;
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="colours"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-tint fa-stack-1x fa-inverse"></span></span> Coloured rows and cells </h4>
  <p>Use contextual classes to color table rows or individual cells.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <table class="table">
            <caption class="wb-inv">
            Table example with colour
            </caption>
            <thead>
              <tr>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr class="active">
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td class="active">Data</td>
              </tr>
              <tr class="success">
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td class="success">Data</td>
              </tr>
              <tr class="warning">
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td class="warning">Data</td>
              </tr>
              <tr class="danger">
                <td>Data Data</td>
                <td>Data Data</td>
              </tr>
              <tr>
                <td>Data Data</td>
                <td class="danger">Data</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li><code>.active</code>: Applies the hover color to a particular row or cell</li>
        <li><code>.success</code>:
          Indicates a successful or positive action</li>
        <li><code>.warning</code>:
          Indicates a warning that might need attention</li>
        <li><code>.danger</code>:
          Indicates a dangerous or potentially negative action</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>//On rows:
&lt;tr <strong>class=&quot;active&quot;</strong>&gt;...&lt;/tr&gt;
&lt;tr <strong>class=&quot;success&quot;</strong>&gt;...&lt;/tr&gt;
&lt;tr <strong>class=&quot;warning&quot;</strong>&gt;...&lt;/tr&gt;
&lt;tr <strong>class=&quot;danger&quot;</strong>&gt;...&lt;/tr&gt;

//On data or header cells ('td' or 'th'):
&lt;tr&gt;
  &lt;td <strong>class=&quot;active&quot;</strong>&gt;...&lt;/td&gt;
  &lt;td <strong>class=&quot;success&quot;</strong>&gt;...&lt;/td&gt;
  &lt;td <strong>class=&quot;warning&quot;</strong>&gt;...&lt;/td&gt;
  &lt;td <strong>class=&quot;danger&quot;</strong>&gt;...&lt;/td&gt;
&lt;/tr&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/tables/tables-en.html" >Data tables</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/charts/charts-en.html" >Charts and graphs</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/zebra/zebra-en.html" >Zebra striping (Advanced)</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/demos/tablevalidator/tablevalidator-en.html" >Table validator</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/demos/equalheight/equalheight-en.html" >Equalize (Equal height)</a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Supporting principles</h2>
  <div data-ajax-replace="../writing/strctr-en.html #tables-info"></div>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
