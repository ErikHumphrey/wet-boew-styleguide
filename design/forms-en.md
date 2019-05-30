---
published: true
layout: default-theme-wet-boew-en
title: Forms
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
                    <li><a href="#labels">Labels</a></li>
                    <li><a href="#inputs">Inputs</a></li>
                    <li><a href="#textarea">Textarea</a></li>
                    <li><a href="#checkboxes">Checkboxes</a></li>
                    <li><a href="#radio">Radio buttons</a></li>
                    <li><a href="#selects">Selects</a></li>
                  </ul>
                </li>
                <li><a href="#enhanced">Enhanced use</a>
                  <ul>
                    <li><a href="#forms-horizontal">Horizontal form</a></li>
                    <li><a href="#forms-inline">Inline form</a></li>
                    <li><a href="#forms-controls-static">Static control</a></li>
                    <li><a href="#forms-control-disabled">Disabled state</a></li>
                    <li><a href="#height">Set height</a></li>
                    <li><a href="#width">Set width</a></li>
										<li><a href="#fieldset">Fieldset/Legend Borders</a></li>
                    <li><a href="#addon">Add-on features</a></li>
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
  <p>Use to collect and transmit information from users in a pre-defined format.</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Design and coding</h2>
  <h3 id="basic">Basic use</h3>
  <p>Use forms with form controls. Individual form controls automatically receive some global styling. All textual <code>&lt;input&gt;</code>, <code>&lt;textarea&gt;</code>, and <code>&lt;select&gt;</code> elements with <code>.form-control</code> are set to <code>width: 100%;</code> by default. Wrap labels and controls in <code>.form-group</code> for optimum spacing.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form method="get" action="#">
            <div class="form-group">
              <label for="exampleInputEmail1">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Enter email" />
            </div>
            <div class="form-group">
              <label for="exampleInputPassword1">Password</label>
              <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password" />
            </div>
            <div class="form-group">
              <label for="exampleInputFile">File input</label>
              <input type="file" id="exampleInputFile" />
            </div>
            <div class="checkbox">
              <label for="checked">
              <input id="checked" type="checkbox" />
              Check me out</label>
            </div>
            <button type="submit" class="btn btn-default">Submit</button>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-8">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <h6>Context for the form:</h6>
      <ul>
        <li>Before including any entry fields for the form,  provide a one line statement about what this form is used for in the following  format:
          <ul>
            <li><strong>Use this form to</strong>…</li>
          </ul>
        </li>
        <li>This assures the user that the form they are  filling out is the correct form</li>
      </ul>
      <h6>Buttons:</h6>
      <ul>
        <li>When placing a<strong> Submit</strong> and <strong>Clear </strong>button at the  end of the form, do not place them next to each other</li>
        <li>Their functions are  the direct opposite of one another, and this could cause unwanted user error due  to proximity of placement</li>
      </ul>
      <h6>Progress bar:</h6>
      <ul>
        <li>When the form is spread over multiple  screens/pages, provide a progress bar to let the user know at what stage in the  completion process they are at</li>
      </ul>
    </div>
    <div class="col-md-12">
      <details>
        <summary>Source code</summary>
        <pre><code>&lt;form role=&quot;form&quot; method=&quot;get&quot; action=&quot;#&quot;&gt;
  &lt;div class=&quot;form-group&quot;&gt;
    &lt;label for=&quot;exampleInputEmail1&quot;&gt;<strong>Email address</strong>&lt;/label&gt;
    &lt;input type=&quot;email&quot; class=&quot;form-control&quot; id=&quot;exampleInputEmail1&quot; placeholder=&quot;Enter email&quot; /&gt;
  &lt;/div&gt;
  &lt;div class=&quot;form-group&quot;&gt;
    &lt;label for=&quot;exampleInputPassword1&quot;&gt;<strong>Password</strong>&lt;/label&gt;
    &lt;input type=&quot;password&quot; class=&quot;form-control&quot; id=&quot;exampleInputPassword1&quot; placeholder=&quot;Password&quot; /&gt;
  &lt;/div&gt;
  &lt;div class=&quot;form-group&quot;&gt;
    &lt;label for=&quot;exampleInputFile&quot;&gt;<strong>File input</strong>&lt;/label&gt;
    &lt;input type=&quot;file&quot; id=&quot;exampleInputFile&quot; /&gt;
  &lt;/div&gt;
  &lt;div class=&quot;checkbox&quot;&gt;
    &lt;label&gt;&lt;input type=&quot;checkbox&quot; /&gt; <strong>Check me out</strong>&lt;/label&gt;
  &lt;/div&gt;
  &lt;button type=&quot;submit&quot; class=&quot;btn btn-default&quot;&gt;<strong>Submit</strong>&lt;/button&gt;
&lt;/form&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="labels"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-left fa-stack-1x fa-inverse"></span></span> Labels</h4>
  <p>Use labels  (a title) to make it clear as to what type of information a user is to enter within an input field. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form >
            <div class="form-group">
              <label for="label-1-0">Label 1</label>
              <input type="text" size="10" id="label-1-0" name="label-1-0" class="form-control" />
            </div>
            <div class="form-group">
              <label for="label-2-0">Label 2</label>
              <input type="password" size="10" id="label-2-0" name="label-2-0" class="form-control" />
            </div>
          </form>
          <h5 class="mrgn-tp-0">Alignment option 1 − Placed  on top </h5>
          <hr>
          <form >
            <div class="form-group">
              <label for="label-1-1">Label 1</label>
              <input type="text" size="10" id="label-1-1" name="label-1-1" class="form-control" />
            </div>
            <div class="form-group">
              <label for="label-2-1">Label 2</label>
              <input type="password" size="10" id="label-2-1" name="label-2-1" class="form-control" />
            </div>
          </form>
          <hr>
          <h5 class="mrgn-tp-0">Alignment option 2 − Aligned right </h5>
          <form action="#" method="get" class="form-horizontal">
            <div class="form-group">
              <label class="col-sm-4 control-label" for="label-1-2">Label 1</label>
              <div class="col-md-8">
                <input type="text" class="form-control" name="label-1-2" id="label-1-2" size="10">
              </div>
            </div>
            <div class="form-group">
              <label class="col-sm-4 control-label" for="label-2-2">Label 2</label>
              <div class="col-md-8">
                <input type="password" class="form-control" name="label-2-2" id="label-2-2" size="10">
              </div>
            </div>
          </form>
          <hr>
          <h5 class="mrgn-tp-0"><span class="glyphicon glyphicon-remove-circle text-danger"></span> Alignment option 3 − Aligned left</h5>
          <form action="#" method="get" class="form-horizontal">
            <div class="form-group">
              <label class="col-sm-4" for="label-1-3">Label 1</label>
              <div class="col-md-8">
                <input type="text" class="form-control" name="label-1-3" id="label-1-3" size="10">
              </div>
            </div>
            <div class="form-group">
              <label class="col-sm-4" for="label-2-3">Label 2</label>
              <div class="col-md-8">
                <input type="password" class="form-control" name="label-2-3" id="label-2-3" size="10">
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-8">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Shorten label text to the essential minimum</li>
        <li>Use sentence case for example, "First name"<strong> not</strong> "First Name"</li>
        <li>Use labels at all times
          <ul>
            <li>Screen readers have trouble with forms if a label is not included for every input</li>
            <li> To hide the label, use the <code>.wb-inv</code> class</li>
          </ul>
        </li>
        <li>Use recognized standard abbreviations, and test abbreviations with non-expert users</li>
        <li>Make a statement rather than  asking a question
          <ul>
            <li>For example, use "Child’s name" instead of "What is the name of the child?"</li>
          </ul>
        </li>
        <li>Use unique label text on any given page to meet accessibility standards</li>
        <li>Place "(required)" at the end of the field label if information is required.  Refer to: <a href="https://wet-boew.github.io/v4.0-ci/docs/ref/formvalid/formvalid-en.html">Form validation</a></li>
      </ul>
      <p class="h6" ><strong>Alignment option 1 design: </strong> </p>
      <ul>
        <li> Place the label <strong>above the input field</strong>. Further  to <a href="https://rosenfeldmedia.com/books/web-form-design/" >Web form design: Filling in the blanks</a>, this is the <strong>recommended</strong> layout
          <ul>
            <li>This layout allows users to  capture both labels and input fields with a single eye movement. While  this is the simplest of layouts, users can process the  information ten times faster than if the information is left-aligned. This is shown in &quot;Alignment option 3 − Left aligned&quot;. This solution uses more vertical  space, but does not impact the user experience. If this does not suit your  specific layout needs &quot;Alignment option 2 − Right aligned&quot; is also <abbr title="O K ">OK</abbr> to use</li>
          </ul>
        </li>
      </ul>
      <p class="h6"><strong>Alignment option 2 design: </strong> </p>
      <ul>
        <li> Place the form objects <strong>side-by-side</strong> only if there is a need to reduce vertical space
          <ul>
            <li>Right align  side-by-side  labels to the form objects.
              This solution is preferred over left  aligned labels. Eye tracking studies  show that  it creates a clear association between label and field. This reduces  the number of fixations the user has (the eye jumping from spot to  spot) by nearly half. As a result, the reduced eye moments and clear  association reduce eye strain, and improve cognition. This translates  to a 50% faster form completion rate</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use a colon at the end of an input field label</li>
        <li>Do not use abbreviations, unless absolutely necessary for space reasons</li>
        <li>Do not abbreviate a critical word.  For example, use "Restricted Acct" not "Rstr Account"</li>
      </ul>
      <p class="h6"><strong>Alignment option 3 design: </strong> </p>
      <ul>
        <li><strong>Do not left-align</strong> a label  from the input field, for the reasons cited above</li>
      </ul>
    </div>
    <div class="col-md-12">
      <details>
        <summary>Source code</summary>
        <pre>
//Alignment option 1 − Placed  on top
&lt;form role=&quot;form&quot;&gt;
   &lt;div class=&quot;form-group&quot;&gt;
     &lt;label for=&quot;label-1-1&quot;&gt;Label 1&lt;/label&gt;
       &lt;input type=&quot;text&quot; size=&quot;10&quot; id=&quot;label-1-1&quot; name=&quot;label-1-1&quot; class=&quot;form-control&quot; /&gt;
   &lt;/div&gt;
   &lt;div class=&quot;form-group&quot;&gt;
     &lt;label for=&quot;label-2-1&quot;&gt;Label 2&lt;/label&gt;
       &lt;input type=&quot;password&quot; size=&quot;10&quot; id=&quot;label-2-1&quot; name=&quot;label-2-1&quot; class=&quot;form-control&quot; /&gt;
    &lt;/div&gt;
&lt;/form&gt;

//Alignment option 2 − Aligned right
&lt;form action=&quot;#&quot; method=&quot;get&quot; role=&quot;form&quot; class=&quot;form-horizontal&quot;&gt;<br>            &lt;div class=&quot;form-group&quot;&gt;
  &lt;label class=&quot;col-sm-4 control-label&quot; for=&quot;label-1-2&quot;&gt;Label 1&lt;/label&gt;
    &lt;div class=&quot;col-md-8&quot;&gt;
       &lt;input type=&quot;text&quot; class=&quot;form-control&quot; name=&quot;label-1-2&quot; id=&quot;label-1-2&quot; size=&quot;10&quot;&gt;
    &lt;/div&gt;
    &lt;/div&gt;
    &lt;div class=&quot;form-group&quot;&gt;
     &lt;label class=&quot;col-sm-4 control-label&quot; for=&quot;label-2-2&quot;&gt;Label 2&lt;/label&gt;
    &lt;div class=&quot;col-md-8&quot;&gt;
       &lt;input type=&quot;password&quot; class=&quot;form-control&quot; name=&quot;label-2-2&quot; id=&quot;label-2-2&quot; size=&quot;10&quot;&gt;
    &lt;/div&gt;
   &lt;/div&gt;
  &lt;/form&gt;</pre>
      </details>
    </div>
	</div>
    <h4 id="inputs"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-square fa-stack-1x fa-inverse"></span></span> Inputs</h4>
    <p>Use text-based input fields (most common form control). This includes support for all HTML5 types: <code>text</code>, <code>password</code>, <code>datetime</code>, <code>datetime-local</code>, <code>date</code>, <code>month</code>, <code>time</code>, <code>week</code>, <code>number</code>, <code>email</code>, <code>url</code>, <code>search</code>, <code>tel</code>, and <code>color</code>.</p>
    <div class="row">
      <div class="col-md-4">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Appearance</h5>
            <h6>Input field</h6>
            <form >
              <input type="text" class="form-control" placeholder="(placeholder text)" />
            </form>
            <form >
              <h6>Input field with a Search button</h6>
              <label for="btngrp-search2" class="wb-inv">Search</label>
              <div class="input-group mrgn-tp-md">
                <input name="text" type="text" class="form-control" id="btngrp-search2" placeholder="(placeholder text)" />
                <span class="input-group-btn">
                <button type="button" class="btn btn-default">Search</button>
                </span></div>
            </form>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Use to create a simple text box that allows for the input of a single line of text</li>
          <li>Declare the <code>type</code> properly − to fully style the input field</li>
          <li> Wrap <code>.input-group-btn</code> around the buttons in input groups
            <ul>
              <li>This is required, as default browser styles cannot be overridden</li>
            </ul>
          </li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
        <p>Compliance point(s):</p>
        <ul>
          <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
          <li>Do not mix form groups directly with input groups
            <ul>
              <li> Instead, nest the input group inside of the form group</li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>// Input field:
&lt;input <strong>type=&quot;text&quot;</strong> class=&quot;form-control&quot; placeholder=&quot;(placeholder text)&quot; /&gt;

// Input field with a Search button:
&lt;label for=&quot;btngrp-search2&quot; class=&quot;wb-inv&quot;&gt;Search&lt;/label&gt;
  &lt;div <strong>class=&quot;input-group&quot;</strong>&gt;
    &lt;input type=&quot;text&quot; class=&quot;form-control&quot; id=&quot;btngrp-search2&quot; placeholder=&quot;(placeholder text)&quot; /&gt;
    &lt;span class=&quot;input-group-btn&quot;&gt;
     &lt;button class=&quot;btn btn-default&quot; type=&quot;button&quot;&gt;Search&lt;/button&gt;
    &lt;/span&gt;
  &lt;/div&gt;</code></pre>
      </div>
    </div>
  </div>
  <h4 id="textarea"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-square fa-stack-1x fa-inverse"></span></span> Textarea</h4>
  <p>Use textareas so users can insert multiple lines of  text within a form. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form method="get" action="#">
            <textarea class="form-control" rows="3"></textarea>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.form-control</code> to create a free-form space that allows the user to type in content</li>
        <li>Change the <code>rows=&quot;*&quot;</code> attribute to reflect the default number of rows to display</li>
        <li>Limit the number of rows to suit the amount of  information that  the recipient(s) desires</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use when users need to enter a specific, pre-defined answer</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;textarea <strong>class=&quot;form-control&quot;</strong> <strong>rows=&quot;3&quot;</strong>&gt;&lt;/textarea&gt;</code></pre>
    </div>
  </div>
  <h4 id="checkboxes"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-check-square fa-stack-1x fa-inverse"></span></span> Checkboxes</h4>
  <p>Use checkboxes so users can select  one <strong>or </strong>several options.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <h6>Default checkboxes</h6>
          <div class="checkbox">
            <label for="defaultCheck1">
            <input id="defaultCheck1" type="checkbox" value="">
            Option 1</label>
          </div>
          <div class="checkbox">
            <label for="defaultCheck2">
            <input id="defaultCheck2" type="checkbox" value="">
            Option 2</label>
          </div>
          <div class="checkbox">
            <label for="defaultCheck3">
            <input id="defaultCheck3" type="checkbox" value="" >
            Option 3</label>
          </div>
          <hr>
          <h6>Inline checkboxes</h6>
          <label for="inlineCheck1" class="checkbox-inline">
          <input id="inlineCheck1" type="checkbox" value="">
          Option 1</label>
          <label for="inlineCheck2" class="checkbox-inline">
          <input id="inlineCheck2" type="checkbox" value="">
          Option 2</label>
          <label for="inlineCheck3" class="checkbox-inline">
          <input id="inlineCheck3" type="checkbox" value="">
          Option 3</label>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.checkbox</code> so users can choose<strong> one or more</strong> predefined set of options</li>
        <li>Use <code>.checkbox-inline</code> to make checkboxes appear on the same line</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use if there is a need for users to enter a detailed answer</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Default checkboxes:
&lt;div <strong>class=&quot;checkbox&quot;</strong>&gt;
   &lt; for=&quot;defaultCheck1&quot; label&gt;&lt;input id=&quot;defaultCheck1&quot; <strong>type=&quot;checkbox&quot;</strong> value=&quot;&quot;&gt;Option 1&lt;/label&gt;
&lt;/div&gt;

// Inline checkboxes:
&lt;div <strong>class=&quot;checkbox-inline&quot;</strong>&gt;
   &lt; for=&quot;inlineCheck1&quot; label&gt;&lt;input id=&quot;inlineCheck1&quot; <strong>type=&quot;checkbox&quot;</strong> value=&quot;&quot;&gt;Option 1&lt;/label&gt;
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="radio"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-circle fa-stack-1x fa-inverse"></span></span> Radio buttons</h4>
  <p>Use radio buttons so users can select  <strong>only one </strong>of several options.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <h6>Radio buttons</h6>
          <div class="radio">
            <label for="radio1">
            <input id="radio1" type="radio" name="optradio">
            Option 1</label>
          </div>
          <div class="radio">
            <label for="radio2">
            <input id="radio2" type="radio" name="optradio">
            Option 2</label>
          </div>
          <div class="radio disabled">
            <label for="radio3">
            <input id="radio3" type="radio" name="optradio" disabled>
            Option 3</label>
          </div>
          <hr>
          <h6>Inline radio buttons</h6>
          <label for="inlineRadio1" class="radio-inline">
          <input id="inlineRadio1" type="radio" name="optradio">
          Option 1</label>
          <label for="inlineRadio2" class="radio-inline">
          <input id="inlineRadio2" type="radio" name="optradio">
          Option 2</label>
          <label for="inlineRadio3" class="radio-inline">
          <input id="inlineRadio3" type="radio" name="optradio">
          Option 3</label>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.radio</code> so users can <strong>only choose one</strong> predefined set of options</li>
        <li>Use <code>.radio-inline</code> to a make radio buttons appear on the same line</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use if there is a need for users to select more than one option</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Radio buttons:
&lt;div <strong>class=&quot;radio&quot;</strong>&gt;
   &lt; for=&quot;radio1&quot;  label&gt;&lt;input id=&quot;radio1&quot; <strong>type=&quot;radio&quot;</strong> name=&quot;optradio&quot;&gt;Option 1&lt;/label&gt;
&lt;/div&gt;

// Inline radio buttons:
&lt;div <strong>class=&quot;radio-inline&quot;</strong>&gt;
   &lt; for=&quot;inlineRadio1&quot; label&gt;&lt;input id=&quot;inlineRadio1&quot; <strong>type=&quot;radio&quot;</strong> name=&quot;optradio&quot;&gt;Option 1&lt;/label&gt;
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="selects"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-caret-square-down fa-stack-1x fa-inverse"></span></span> Selects</h4>
  <p>Use so users can select<strong> only one </strong>of several options from within a list. A single item in a dropdown list, or multiple options can display at once. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <h6>Dropdown list with single option view</h6>
          <form method="get" action="#">
            <select class="form-control">
              <option>1</option>
              <option>2</option>
              <option>3</option>
              <option>4</option>
              <option>5</option>
            </select>
            <hr>
            <h6>Dropdown list with multi-option view</h6>
            <select multiple="multiple" class="form-control">
              <option>1</option>
              <option>2</option>
              <option>3</option>
              <option>4</option>
              <option>5</option>
            </select>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Correct use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Use <code>.form-control</code> to create a selection list, from which the user can select a single option</li>
        <li>Add <code>multiple</code> to show multiple options at once</li>
        <li>Place the most likely  select option as the default dropdown text</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Incorrect use</h5>
      <p>Compliance point(s):</p>
      <ul>
        <li>Do not use this component in a way that conflicts with the preceding compliance <span class="nowrap">point(s)</span></li>
        <li>Do not use for non-related items</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Dropdown list with single option view:
&lt;select <strong>class=&quot;form-control&quot;</strong>&gt;
&lt;option&gt;1&lt;/option&gt;
&lt;option&gt;2&lt;/option&gt;
&lt;option&gt;3&lt;/option&gt;
&lt;option&gt;4&lt;/option&gt;
&lt;option&gt;5&lt;/option&gt;
&lt;/select&gt;

// Dropdown list with multi-option view:
&lt;select <strong>multiple=&quot;multiple&quot; class=&quot;form-control&quot;</strong>&gt;
&lt;option&gt;1&lt;/option&gt;
&lt;option&gt;2&lt;/option&gt;
&lt;option&gt;3&lt;/option&gt;
&lt;option&gt;4&lt;/option&gt;
&lt;option&gt;5&lt;/option&gt;
&lt;/select&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Enhanced use</h3>
  <h4 id="forms-horizontal"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-th-list fa-stack-1x fa-inverse"></span></span> Horizontal form</h4>
  <p>Use Bootstrap's predefined grid classes to align labels and groups of form controls in a horizontal layout by adding <code>.form-horizontal</code> to the form. Doing so changes a <code>.form-group</code> to behave as a grid row. So there is no need for <code>.row</code>.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form class="form-horizontal" method="get" action="#">
            <div class="form-group">
              <label for="inputEmail3" class="col-sm-4 control-label">Email</label>
              <div class="col-sm-8">
                <input type="email" class="form-control" id="inputEmail3" placeholder="Email" />
              </div>
            </div>
            <div class="form-group">
              <label for="inputPassword3" class="col-sm-4 control-label">Password</label>
              <div class="col-sm-8">
                <input type="password" class="form-control" id="inputPassword3" placeholder="Password" />
              </div>
            </div>
            <div class="form-group">
              <div class="col-sm-offset-4 col-sm-8">
                <div class="checkbox">
                  <label for="remember1">
                  <input id="remember1" type="checkbox" />
                  Remember me</label>
                </div>
              </div>
            </div>
            <div class="form-group">
              <div class="col-sm-offset-4 col-sm-8">
                <button type="submit" class="btn btn-default">Sign in</button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-8">
      <details>
        <summary>Source code</summary>
        <pre><code>&lt;form <strong>class=&quot;form-horizontal&quot;</strong> role=&quot;form&quot; method=&quot;get&quot; action=&quot;#&quot;&gt;
  &lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
	&lt;label for=&quot;inputEmail3&quot; class=&quot;col-sm-2 control-label&quot;&gt;<strong>Email</strong>&lt;/label&gt;
	&lt;div class=&quot;col-sm-10&quot;&gt;
		&lt;input type=&quot;email&quot; class=&quot;form-control&quot; id=&quot;inputEmail3&quot; placeholder=&quot;Email&quot; /&gt;
	&lt;/div&gt;
  &lt;/div&gt;
 &lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
	&lt;label for=&quot;inputPassword3&quot; class=&quot;col-sm-2 control-label&quot;&gt;<strong>Password</strong>&lt;/label&gt;
	&lt;div class=&quot;col-sm-10&quot;&gt;
		&lt;input type=&quot;password&quot; class=&quot;form-control&quot; id=&quot;inputPassword3&quot; placeholder=&quot;Password&quot; /&gt;
	&lt;/div&gt;
  &lt;/div&gt;
  &lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
	&lt;div class=&quot;col-sm-offset-2 col-sm-10&quot;&gt;
		&lt;div class=&quot;checkbox&quot;&gt;
			&lt; for=&quot;remember1&quot; label&gt;&lt;input id=&quot;remember1&quot; type=&quot;checkbox&quot; /&gt; <strong>Remember me</strong>&lt;/label&gt;
		&lt;/div&gt;
	&lt;/div&gt;
  &lt;/div&gt;
  &lt;div<strong> class=&quot;form-group&quot;</strong>&gt;
	&lt;div class=&quot;col-sm-offset-2 col-sm-10&quot;&gt;
		&lt;button type=&quot;submit&quot; class=&quot;btn btn-default&quot;&gt;<strong>Sign in</strong>&lt;/button&gt;
	&lt;/div&gt;
  &lt;/div&gt;
&lt;/form&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="forms-inline"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ellipsis-h fa-stack-1x fa-inverse"></span></span> Inline  form</h4>
  <p>Use the inline form,  and set a width on the form controls.   For a compact layout, add <code>.form-inline</code> for left-aligned and inline-block controls. Inputs, selects, and textareas are 100% wide by default in Bootstrap.</p>
  <div class="row">
    <div class="col-md-8">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form class="form-inline" method="get" action="#">
            <div class="form-group">
              <label class="wb-inv" for="exampleInputEmail2">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail2" placeholder="Enter email" />
            </div>
            <div class="form-group">
              <label class="wb-inv" for="exampleInputPassword2">Password</label>
              <input type="password" class="form-control" id="exampleInputPassword2" placeholder="Password" />
            </div>
            <div class="checkbox">
              <label for="remember2">
              <input id="remember2" type="checkbox" />
              Remember me</label>
            </div>
            <button type="submit" class="btn btn-default">Sign in</button>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <details>
        <summary>Source code</summary>
        <pre><code>&lt;form <strong>class=&quot;form-inline&quot; </strong>role=&quot;form&quot; method=&quot;get&quot; action=&quot;#&quot;&gt;
  &lt;div class=&quot;form-group&quot;&gt;
	&lt;label class=&quot;wb-inv&quot; for=&quot;exampleInputEmail2&quot;&gt;Email address&lt;/label&gt;
	&lt;input type=&quot;email&quot; class=&quot;form-control&quot; id=&quot;exampleInputEmail2&quot; placeholder=&quot;Enter email&quot; /&gt;
  &lt;/div&gt;
  &lt;div class=&quot;form-group&quot;&gt;
	&lt;label class=&quot;wb-inv&quot; for=&quot;exampleInputPassword2&quot;&gt;Password&lt;/label&gt;
	&lt;input type=&quot;password&quot; class=&quot;form-control&quot; id=&quot;exampleInputPassword2&quot; placeholder=&quot;Password&quot; /&gt;
  &lt;/div&gt;
  &lt;div class=&quot;checkbox&quot;&gt;
	&lt; for=&quot;remember2&quot; label&gt;&lt;input id=&quot;remember2&quot; type=&quot;checkbox&quot; /&gt; Remember me&lt;/label&gt;
  &lt;/div&gt;
  &lt;button type=&quot;submit&quot; class=&quot;btn btn-default&quot;&gt;Sign in&lt;/button&gt;
&lt;/form&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4  id="forms-controls-static"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="glyphicon glyphicon-eye-open fa-stack-1x fa-inverse"></span></span> Static control</h4>
  <p>Use when there is a need to place a read-only field in the form, use <code>readonly="readonly"</code>.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form class="form-horizontal" method="get" action="#">
            <div class="form-group">
              <label for="emailReadonly" class="col-sm-4 control-label">Email</label>
              <div class="col-sm-8">
                <input type="email" readonly id="emailReadonly" value="email@example.com" />
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-8">
      <details>
        <summary>Source code</summary>
        <pre><code>&lt;form class=&quot;form-horizontal&quot; role=&quot;form&quot; method=&quot;get&quot; action=&quot;#&quot;&gt;
  &lt;div class=&quot;form-group&quot;&gt;
	&lt;label for=&quot;emailReadonly&quot; class=&quot;col-sm-2 control-label&quot;&gt;Email&lt;/label&gt;
	&lt;div class=&quot;col-sm-10&quot;&gt;
		&lt;input type=&quot;email<strong>&quot; readonly=&quot;readonly&quot;</strong> id=&quot;emailReadonly&quot; value=&quot;email@example.com&quot; /&gt;
	&lt;/div&gt;
  &lt;/div&gt;
&lt;/form&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="forms-control-disabled"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Disabled state</h4>
  <p>Use to to prevent user input, and to trigger a slightly different look. Add <code>disabled="disabled"</code> to an input field.</p>
  <p>Add the <code>disabled</code> attribute to a <code>&lt;fieldset&gt;</code> to disable all the controls within the <code>&lt;fieldset&gt;</code> at once.</p>
  <p>Link functionality of <code>&lt;a&gt;</code> is not impacted. This class only changes the appearance of <code>&lt;a class="btn btn-default"&gt;</code> buttons, not their functionality. Use custom JavaScript to disable links here.</p>
  <p><strong>Cross-browser compatibility: </strong>While Bootstrap applies these styles in all browsers, Internet Explorer 9 and below don't actually support the <code>disabled</code> attribute on a <code>&lt;fieldset&gt;</code>. Apply <code>disabled="disabled"</code> to all the fields contained within the disabled fieldset to fix the issue in these browsers.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form method="get" action="#">
            <fieldset disabled>
            <div class="form-group">
              <label for="disabledTextInput">Disabled input</label>
              <input type="text" id="disabledTextInput" class="form-control" placeholder="Disabled input" />
            </div>
            <div class="form-group">
              <label for="disabledSelect">Disabled select menu</label>
              <select id="disabledSelect" class="form-control">
                <option>Disabled select</option>
              </select>
            </div>
            <div class="checkbox">
              <label for="unchecked">
              <input id="unchecked" type="checkbox" />
              Can't check this</label>
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
            </fieldset>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-8">
      <details>
        <summary>Source code</summary>
        <pre><code>&lt;form role=&quot;form&quot; method=&quot;get&quot; action=&quot;#&quot;&gt;
  &lt;fieldset <strong>disabled=&quot;disabled&quot;</strong>&gt;
	&lt;div class=&quot;form-group&quot;&gt;
		&lt;label for=&quot;disabledTextInput&quot;&gt;Disabled input&lt;/label&gt;
		&lt;input type=&quot;text&quot; id=&quot;disabledTextInput&quot; class=&quot;form-control&quot; placeholder=&quot;Disabled input&quot; /&gt;
	&lt;/div&gt;
	&lt;div class=&quot;form-group&quot;&gt;
		&lt;label for=&quot;disabledSelect&quot;&gt;Disabled select menu&lt;/label&gt;
		&lt;select id=&quot;disabledSelect&quot; class=&quot;form-control&quot;&gt;
			&lt;option&gt;Disabled select&lt;/option&gt;
		&lt;/select&gt;
	&lt;/div&gt;
	&lt;div class=&quot;checkbox&quot;&gt;
		&lt; for=&quot;unchecked&quot; label&gt;
		&lt;input id=&quot;unchecked&quot; type=&quot;checkbox&quot; /&gt; Can&#39;t check this&lt;/label&gt;
	&lt;/div&gt;
	&lt;button type=&quot;submit&quot; class=&quot;btn btn-primary&quot;&gt;Submit&lt;/button&gt;
  &lt;/fieldset&gt;
&lt;/form&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="height"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-v fa-stack-1x fa-inverse"></span></span> Set height</h4>
  <p>Use to create larger or smaller form controls that match button sizes with the classes <code>.input-lg</code> or <code>.input-sm</code>. Medium is the default  size. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form method="get" action="#">
            <div class="controls">
              <label for="form-input-lg" class="wb-inv"><code>input-lg</code> class on an input element</label>
              <input name="text2" type="text" class="form-control input-lg mrgn-bttm-md" id="form-input-lg" placeholder="input-lg" />
              <label for="form-input-md" class="wb-inv">Default input element</label>
              <input type="text" class="form-control mrgn-bttm-md" id="form-input-md" placeholder="Default input" />
              <label for="form-input-sm" class="wb-inv"><code>input-sm</code> class on an input element</label>
              <input class="form-control input-sm mrgn-bttm-md" type="text" id="form-input-sm" placeholder="input-sm" />
              <label for="form-select-lg" class="wb-inv"><code>input-lg</code> class on a select element</label>
              <select class="form-control input-lg mrgn-bttm-md" id="form-select-lg">
                <option value="">.input-lg</option>
              </select>
              <label for="form-select-md" class="wb-inv">Default select element</label>
              <select class="form-control mrgn-bttm-md" id="form-select-md">
                <option value="">Default select</option>
              </select>
              <label for="form-select-sm" class="wb-inv"><code>input-sm</code> class on a select element</label>
              <select class="form-control input-sm mrgn-bttm-md" id="form-select-sm">
                <option value="">.input-sm</option>
              </select>
            </div>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-8">
      <details>
        <summary>Source code</summary>
        <pre><code>&lt;label for=&quot;form-input-lg&quot; class=&quot;wb-inv&quot;&gt;&lt;code&gt;input-lg&lt;/code&gt; class on an input element&lt;/label&gt;
&lt;input name=&quot;text2&quot; type=&quot;text&quot; class=&quot;form-control <strong>input-lg</strong> mrgn-bttm-md&quot; id=&quot;form-input-lg&quot; placeholder=&quot;input-lg&quot; /&gt;

&lt;label for=&quot;form-input-md&quot; class=&quot;wb-inv&quot;&gt;Default input element&lt;/label&gt;
&lt;input type=&quot;text&quot; class=&quot;form-control mrgn-bttm-md&quot; id=&quot;form-input-md&quot; placeholder=&quot;<strong>Default</strong> input&quot; /&gt;

&lt;label for=&quot;form-input-sm&quot; class=&quot;wb-inv&quot;&gt;&lt;code&gt;input-sm&lt;/code&gt; class on an input element&lt;/label&gt;
&lt;input class=&quot;form-control <strong>input-sm </strong>mrgn-bttm-md&quot; type=&quot;text&quot; id=&quot;form-input-sm&quot; placeholder=&quot;input-sm&quot; /&gt;


&lt;label for=&quot;form-select-lg&quot; class=&quot;wb-inv&quot;&gt;&lt;code&gt;input-lg&lt;/code&gt; class on a select element&lt;/label&gt;
   &lt;select class=&quot;form-control <strong>input-lg</strong> mrgn-bttm-md&quot; id=&quot;form-select-lg&quot;&gt;
      &lt;option value=&quot;&quot;&gt;.input-lg&lt;/option&gt;
&lt;/select&gt;

&lt;label for=&quot;form-select-md&quot; class=&quot;wb-inv&quot;&gt;Default select element&lt;/label&gt;
   &lt;select class=&quot;form-control mrgn-bttm-md&quot; id=&quot;form-select-md&quot;&gt;
      &lt;option value=&quot;&quot;&gt;<strong>Default</strong> select&lt;/option&gt;
   &lt;/select&gt;

&lt;label for=&quot;form-select-sm&quot; class=&quot;wb-inv&quot;&gt;&lt;code&gt;input-sm&lt;/code&gt; class on a select element&lt;/label&gt;
   &lt;select class=&quot;form-control <strong>input-sm</strong> mrgn-bttm-md&quot; id=&quot;form-select-sm&quot;&gt;
      &lt;option value=&quot;&quot;&gt;.input-sm&lt;/option&gt;
   &lt;/select&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="width"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-h fa-stack-1x fa-inverse"></span></span> Set width</h4>
  <p>Use to wrap inputs in grid columns such as <code>.col-xs-4</code> or <code>.col-xs-8</code> (or any custom parent element) to easily enforce desired widths.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <form method="get" action="#">
            <div class="row">
              <div class="col-xs-4">
                <label for="form-input-col-xs-4" class="wb-inv"><code>col-xs-4</code> class on the parent element</label>
                <input type="text" class="form-control" id="form-input-col-xs-4" placeholder="col-xs-4" />
              </div>
              <div class="col-xs-8">
                <label for="form-input-col-xs-8" class="wb-inv"><code>col-xs-8</code> class on the parent element</label>
                <input type="text" class="form-control" id="form-input-col-xs-8" placeholder="col-xs-8" />
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
    <div class="col-md-8">
      <details>
        <summary>Source code</summary>
        <pre><code>&lt;div class=&quot;row&quot;&gt;
  &lt;div<strong> class=&quot;col-xs-4&quot;</strong>&gt;
	&lt;label for=&quot;form-input-col-xs-4&quot; class=&quot;wb-inv&quot;&gt;&lt;code&gt;col-xs-4&lt;/code&gt; class on the parent element&lt;/label&gt;
	&lt;input type=&quot;text&quot; class=&quot;form-control&quot; id=&quot;form-input-col-xs-4&quot; placeholder=&quot;col-xs-4&quot; /&gt;
  &lt;/div&gt;
  &lt;div<strong> class=&quot;col-xs-8&quot;</strong>&gt;
	&lt;label for=&quot;form-input-col-xs-8&quot; class=&quot;wb-inv&quot;&gt;&lt;code&gt;col-xs-8&lt;/code&gt; class on the parent element&lt;/label&gt;
	&lt;input type=&quot;text&quot; class=&quot;form-control&quot; id=&quot;form-input-col-xs-8&quot; placeholder=&quot;col-xs-8&quot; /&gt;
  &lt;/div&gt;
&lt;/div&gt;</code></pre>
      </details>
    </div>
  </div>
	<h4 id="fieldset"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span></span> Fieldsets Borders</h4>
	<p>By default a single <code>fieldset/legend</code> has no top border. Each fieldset after the first <code>fieldset/legend</code> well have a border to sperate the two fieldsets. This can be changed by using <code>.legend-brdr-bttm</code> class on the <code>&lt;fieldset&gt;</code> to create a border under each <code>&lt;legend&gt;</code>.</p>
	<div class="row">
	  <div class="col-md-4">
	    <div class="panel panel-default">
	      <div class="panel-body">
	        <h5 class="mrgn-tp-0">Appearance</h5>
	        <form class="form-horizontal" method="get" action="#">
	          <fieldset class="legend-brdr-bttm">
	            <legend>Identification Information</legend>
	            <div class="form-group">
	              <label for="inputFullName" class="col-sm-4 control-label">Full Name</label>
	              <div class="col-sm-8">
	                <input type="text" class="form-control" id="inputFullName" placeholder="Full Name" />
	              </div>
	            </div>
							<div class="form-group">
								<label for="dob" class="col-sm-4 control-label">Date of Birth <span class="datepicker-format"> (YYYY-MM-DD)</span></label>
								<div class="col-sm-8">
									<input class="form-control" id="dob" name="dob" type="date" />
								</div>
							</div>
	          </fieldset>
						<fieldset class="legend-brdr-bttm">
							<legend>Contact Information</legend>
							<div class="form-group">
								<label for="tel1" class="col-sm-4 control-label">Telephone number</label>
								<div class="col-sm-8">
									<input class="form-control" id="tel1" name="tel1" type="tel" />
								</div>
							</div>
							<div class="form-group">
	              <label for="inputEmail4" class="col-sm-4 control-label">Email</label>
	              <div class="col-sm-8">
	                <input type="email" class="form-control" id="inputEmail4" placeholder="Email" />
	              </div>
	            </div>
						</fieldset>
	          <div class="form-group">
	            <div class="col-sm-offset-4 col-sm-8">
	              <button type="submit" class="btn btn-default">Sign Up</button>
	            </div>
	          </div>
	        </form>
	      </div>
	    </div>
	  </div>
	  <div class="col-md-8">
	    <details>
	      <summary>Source code</summary>
	      <pre><code>&lt;form <strong>class=&quot;form-horizontal&quot;</strong> role=&quot;form&quot; method=&quot;get&quot; action=&quot;#&quot;&gt;
&lt;fieldset <strong>class=&quot;legend-brdr-bttm&quot;</strong>&gt;
	&lt;legend&gt;<strong>Identification Information</strong>&lt;/legend&gt;
	&lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
		&lt;label for=&quot;inputFullName&quot; class=&quot;col-sm-4 control-label&quot;&gt;<strong>Full Name</strong>&lt;/label&gt;
		&lt;div class="col-sm-8"&gt;
		&lt;input type=&quot;text&quot; class=&quot;form-control&quot; id=&quot;inputFullName&quot; placeholder=&quot;Full Name&quot; /&gt;
		&lt;/div&gt;
	&lt;/div&gt;
	&lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
		&lt;label for=&quot;dob&quot; class=&quot;col-sm-4 control-label&quot;&gt;<strong>Date of Birth</strong>&lt;span  <strong>class=&quot;datepicker-format&quot;&gt;</strong> (YYYY-MM-DD)&lt;/span&gt;&lt;/label&gt;
		&lt;div class="col-sm-8"&gt;
		&lt;input class=&quot;form-control&quot; id=&quot;dob&quot; name=&quot;dob&quot; type=&quot;date&quot; /&gt;
		&lt;/div&gt;
	&lt;/div&gt;
&lt;/fieldset&gt;
&lt;fieldset <strong>class=&quot;legend-brdr-bttm&quot;</strong>&gt;
	&lt;legend&gt;<strong>Contact Information</strong>&lt;/legend&gt;
	&lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
		&lt;label for=&quot;tel1&quot; class=&quot;col-sm-4 control-label&quot;&gt;<strong>Telephone number</strong>&lt;/label&gt;
		&lt;div class=&quot;col-sm-8&quot;&gt;
		&lt;input class=&quot;form-control&quot; id=&quot;tel1&quot; name=&quot;tel1&quot; type=&quot;tel&quot; /&gt;
		&lt;/div&gt;
	&lt;/div&gt;
	&lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
		&lt;label for=&quot;inputEmail3&quot; class=&quot;col-sm-4 control-label&quot;&gt;<strong>Email</strong>&lt;/label&gt;
		&lt;div class=&quot;col-sm-8&quot;&gt;
		&lt;input type=&quot;email&quot; class=&quot;form-control&quot; id=&quot;inputEmail3&quot; placeholder=&quot;Email&quot; /&gt;
		&lt;/div&gt;
	&lt;/div&gt;
&lt;/fieldset&gt;
&lt;div <strong>class=&quot;form-group&quot;</strong>&gt;
	&lt;div class=&quot;col-sm-offset-2 col-sm-10&quot;&gt;
		&lt;button type=&quot;submit&quot; class=&quot;btn btn-default&quot;&gt;<strong>Sign in</strong>&lt;/button&gt;
	&lt;/div&gt;
&lt;/div&gt;
&lt;/form&gt;</code></pre>
	      </details>
	    </div>
	  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Add-on features</h4>
  <p>Additional add-on features and behaviours are available.</p>
  <ul class="list-inline lst-spcd">
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/datalist/datalist-en.html"  class="btn btn-default">Datalist (autocomplete) </a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/datalist/datalist-en.html"  class="btn btn-default">Datalist (autocomplete) − Dynamic</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/datepicker/datepicker-en.html"  class="btn btn-default">Date picker </a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/formvalid/formvalid-en.html"  class="btn btn-default">Forms validation</a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Some of the code and documentation for this page is sourced from <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (external link)</span></a></p>
{% endraw %}
{:/}
