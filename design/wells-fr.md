---
published: true
layout: default-theme-wet-boew-fr
title: Boîte grisonné
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
          <h2 class="panel-title">Table des matières</h2>
        </header>
        <div class="panel-body">
          <ul>
            <li><a href="#purpose">Usage</a></li>
            <li><a href="#design">Conception et codage</a>
              <ul>
                <li><a href="#basic">Utilisation de base</a>
                  <ul>
                    <li><a href="#default">Défaut</a></li>
                    <li><a href="#small">Petit « well » </a></li>
                    <li><a href="#large">Grand « well » </a></li>
                  </ul>
                </li>
                <li><a href="#enhanced">Utilisation améliorée</a>
                  <ul>
                    <li><a href="#addon">Fonctions complémentaires</a> </li>
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
          <h2 class="mrgn-tp-0 h4 text-warning"><span class="fa fa-exclamation-triangle"></span> Chantier</h2>
          <p>Cette page est en chantier.</p>
          <p>Veuillez <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage</h2>
  <p>Les utiliser pour mettre un élément de contenu en évidence en le plaçant dans une case de couleur gris clair.</p>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base</h3>

  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Défaut</h4>
  <p>Utilisez la taille du « well » par défaut dans la plupart des situations. </p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="well">Contenu</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
<p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>L'utiliser pour attirer l'attention sur un segment particulier présentant au contenu digne de mention</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5><p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">le point</span>  d'observation  <span class="nowrap">précédent</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class=&quot;well&quot;</strong>&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="small"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-compress fa-stack-1x fa-inverse"></span></span> Petit « well »</h4>
  <p>Utilisez le petit « well » lorsque l'espace est précieux et que la réduction du remplissage intérieur permet de faire apparaître plus de contenu dans une seule rangée.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="well well-sm">Contenu</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
<p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.well-sm</code> pour attirer l'attention sur un segment particulier présentant au contenu digne de mention, en plus de réduire le remplissage interne du conteneur</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5><p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">le point</span>  d'observation  <span class="nowrap">précédent</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class=&quot;well well-sm&quot;</strong>&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="large"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-expand fa-stack-1x fa-inverse"></span></span> Grand « well »</h4>
  <p>Utilisez le grand  « well » lorsqu'il faut plus de visibilité dans la page. Puisque le « well » par défaut assure déjà une visibilité, il est peu utile d'utiliser un « well » plus grand.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="well well-lg">Contenu</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
<p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.well-lg</code> pour attirer l'attention sur un segment particulier présentant au contenu digne de mention, en plus d'élargir le remplissage interne du conteneur</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5><p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">le point</span>  d'observation  <span class="nowrap">précédent</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class=&quot;well well-lg&quot;</strong>&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Utilisation améliorée</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires</h4>
  <p>Des caractéristiques et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/equalheight/equalheight-fr.html"  class="btn btn-default">Égalisation (égalisation des hauteurs)</a></li>
    <li><a href="proximity-fr.html" class="btn btn-default">Proximité des marges </a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
