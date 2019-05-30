---
published: true
layout: default-theme-wet-boew-fr
title: Bordures
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
          <h2 class="panel-title">Table des matières </h2>
        </header>
        <div class="panel-body">
          <ul>
            <li><a href="#purpose">Usage</a></li>
            <li><a href="#design">Conception et condage </a>
              <ul>
                <li><a href="#basic">Utilisation de base </a> </li>
                <li><a href="#enhanced">Utilisation améliorée </a>
                  <ul>
                    <li><a href="#hr">Règle horizontale <code>&lt;hr&gt;</code></a></li>
                    <li><a href="#radius">Remove border radius</a></li>
                    <li><a href="#addon">Fonctions complémentaires </a></li>
                  </ul>
                </li>
              </ul>
            </li>
            <li><a href="#supporting">Principes de soutien </a></li>
          </ul>
        </div>
      </div>
    </nav>
    <section class="col-md-4">
      <div class="panel panel-warning">
        <div class="panel-body">
          <h2 class="mrgn-tp-0 h4 text-warning"><span class="fa fa-exclamation-triangle"></span> Travail en cours</h2>
          <p>Cette page porte sur le travail en cours.</p>
          <p>Veuillez  <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage </h2>
  <p>Utilisez pour ajouter une ou plusieurs bordures afin de concevoir des éléments afin de séparer  ou y attirer l'attention sur le contenu. De plus, retirez les bordures par défaut ou taillez les coins qui semblent être dans les éléments de conception tels qu'un «&nbsp;puits&nbsp;». </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage </h2>
  <h3 id="basic">Utilisation de base </h3>
  <h4 id="left"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-270">&macr;&macr;&macr;</span></span> Bordure gauche</h4>
  <p>Utilisez pour ajouter une bordure gauche à un élément. Si elle est appliquée à des grilles, la bordure s'affiche sur le bord extérieur de la gouttière 15px.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="col-md-12 brdr-lft"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.brdr-lft</code> pour ajouter une bordure gauche</li>
        <li>Utilisez pour séparer le contenu</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
     <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-lft</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="right"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-90">&macr;&macr;&macr;</span></span>Bordure droite </h4>
  <p>Utilisez pour ajouter une bordure droite à l'élément. Si elle est appliquée à des grilles, la bordure s'affiche sur le bord extérieur de la gouttière 15px.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="col-md-12 brdr-rght"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation  </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.brdr-rght</code> pour ajouter une bordure droite</li>
        <li>Utilisez pour séparer le contenu</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-rght</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="top"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&macr;&macr;&macr;</span></span> Bordure supérieure</h4>
  <p>Utilisez une bordure supérieure à un élément. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="col-md-12 brdr-tp"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation  </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.brdr-tp</code> pour ajouter une bordure supérieure</li>
        <li>Utilisez pour séparer le contenu</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-tp</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="bottom"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-180">&macr;&macr;&macr;</span></span> Bordure inférieure </h4>
  <p>Utilisez pour ajouter une bordure inférieure à un élément.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="col-md-12 brdr-bttm"><br>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.brdr-bttm</code> pour ajouter une bordure inférieure</li>
        <li>Utilisez pour séparer le contenu</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation  </h5>
      <p>Point d'observation&nbsp;:</p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div class=&quot;col-md-12 <strong>brdr-bttm</strong>&quot;&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Utilisation améliorée </h3>
  <h4 id="hr"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse fa-rotate-180">&macr;&macr;&macr;</span></span> Règle horizontale <code>&lt;hr&gt;</code></h4>
  <p>Utilisez pour appliquer une bordure à  <code>&lt;hr&gt;</code> pour l'obscurcir.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Par défaut :</p>
          <hr>
          <p>Obscurci :</p>
          <hr class="brdr-bttm">
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation  </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>Utilisez pour définir un changement thématique au contenu, selon l'usage approprié de <code>&lt;hr&gt;</code></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation  </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Défaut :
<strong>&lt;hr&gt;</strong>

// Raccourci&nbsp;:
&lt;hr <strong>class=&quot;brdr-bttm&quot;</strong>&gt;</code></pre>
    </div>
  </div>
  <h4 id="radius"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&lceil;</span></span> Retirer un rayon de bordure </h4>
  <p>Utilisez pour retirer le rayon de bordure à partir d'une composante de conception, comme un <a href="wells-fr.html">puits</a>.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="row">
            <div class="col-sm-6">
              <div class="well">
                <p>Défaut</p>
              </div>
            </div>
            <div class="col-sm-6">
              <div class="well brdr-rds-0">
                <p>Aucun rayon </p>
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col-sm-6">
              <div class="panel panel-default">
                <div class="panel-heading">
                  <h5 class="panel-title">Défaut</h5>
                </div>
                <div class="panel-body"> </div>
              </div>
            </div>
            <div class="col-sm-6">
              <div class="panel panel-default brdr-rds-0">
                <div class="panel-heading">
                  <h5 class="panel-title">Aucun rayon </h5>
                </div>
                <div class="panel-body"> </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation  </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>Utilisez  <code>.brdr-rds-0</code> afin de retirer le rayon d'une bordure dans un  panneau ou un puits</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Aucun rayon dans un panneau :
&lt;div <strong>class=&quot;brdr-rds-0 </strong>panel panel-default&quot;&gt;
...
&lt;/div&gt;

// Aucun rayon dans un puits:
&lt;div <strong>class=&quot;brdr-rds-0</strong> well&quot;&gt;
...
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires </h4>
  <p> Des fonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/equalheight/equalheight-fr.html" >Égaliser (égalisation des hauteurs)</a></li>
  </ul>
  <h2 id="supporting" tabindex="-1"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Principes de soutien </h2>
  <p> Selon le principe de la région commune, les objets se trouvant dans la même région délimitée (bordée) sont perçus comme regroupés. </p>
{% endraw %}
{:/}
