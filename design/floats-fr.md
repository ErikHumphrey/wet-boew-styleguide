---
published: true
layout: default-theme-wet-boew-fr
title: Éléments flottants
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
            <li> <a href="#design">Conception et codage</a>
              <ul>
                <li> <a href="#basic">Utilisation de base</a>
                  <ul>
                    <li><a href="#right">Éléments flottants de droite</a></li>
                    <li> <a href="#left">Éléments flottants de gauche</a></li>
                    <li><a href="#clearing">Éléments flottants d'écrasement</a></li>
                  </ul>
                </li>
                <li><a href="#enhanced">Utilisation améliorée</a>
                  <ul>
                    <li><a href="#addon">Fonctions complétementaires</a></li>
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
          <p>Veuillez  <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a>  ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span>Usage</h2>
  <p>Utilisez un élément flottant pour changer le flux normal d'un élément. Repoussez l'élément à droite ou à gauche de son conteneur, où le texte et les éléments incorporés  l'enveloppent. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base </h3>
  <h4 id="right"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-arrow-right fa-stack-1x fa-inverse"></span></span> Éléments flottants de droite</h4>
  <p>Servent à faire flotter un élément vers la droite.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="pull-right">Tiré à droite</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.pull-right</code> pour faire flotter un élément de contenu particulier à droite tandis que des éléments non flottants l'enveloppent</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
        <li>N'utilisez pas cet élément pour aligner du texte à droite. Pour les options d'alignement, consultez : <a href="alignment-fr.html">Alignement</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class=&quot;pull-right&quot;</strong>&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="left"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-arrow-left fa-stack-1x fa-inverse"></span></span> Éléments flottants de gauche</h4>
  <p>Servent à faire flotter un élément vers la gauche.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="pull-left">Tiré à gauche</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
<p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>Utilisez <code>.pull-left</code> pour faire flotter un élément de contenu particulier à gauche tandis que des éléments non flottants l'enveloppent</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p><ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
        <li>N'utilisez pas cet élément pour aligner du texte à gauche.  Pour les options d'alignement, consultez : <a href="/english/r1713497special/chad_crf000/styleguide-new/theme-wet-boew/design/alignment-fr.html">Alignement</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class=&quot;pull-left&quot;</strong>&gt;...&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="clearing"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Éléments flottants d'écrasement</h4>
  <p>Utilisez ces éléments pour écraser (réinitialiser) l'élément flottant de contenu sur n'importe quel élément.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Sans écrasement :</p>
          <p class="pull-right mrgn-lft-md">Tiré à droite A</p>
          <p class="pull-right">Tiré à droite B</p>
          <div class="clearfix"></div>
          <p>Avec écrasement :</p>
          <p class="pull-right">Tiré à droite A</p>
          <div class="clearfix"></div>
          <p class="pull-right">Tiré à droite B</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation</span>&nbsp;:</p>
        <ul>
        <li>Utilisez <code>.clearfix</code> pour réinitialiser le flux de contenu et empêcher que d'autres éléments de contenu ne flottent autour ou au-dessus d'un élément</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation</span>&nbsp;:</p>
      <ul>
       <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p class=&quot;pull-right&quot;&gt;Tiré à droite A&lt;/p&gt;<br>&lt;div <strong>class=&quot;clearfix&quot;</strong>&gt;&lt;/div&gt;<br>&lt;p class=&quot;pull-right&quot;&gt;Tiré à droite B&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Utilisation améliorée</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Caractéristiques complémentaires</h4>
  <p>Des fonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="reflow-fr.html">Redistribution du contenu autour de grilles</a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" rel="external">Bootstrap<span class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
