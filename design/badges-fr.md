---
published: true
layout: default-theme-wet-boew-fr
title: Badges
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
                <li><a href="#basic">Utilisation de base</a> </li>
                <li><a href="#enhanced">Utilisation améliorée </a>
                  <ul>
                    <li><a href="#collapsing">Badges qui se réduisent seuls </a></li>
                    <li><a href="#addon">Fonctions complémentaires </a> </li>
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
          <h2 class="mrgn-tp-0 h4 text-warning"><span class="fa fa-exclamation-triangle"></span> Travail en cours </h2>
          <p>Cette  page porte sur le travail en cours.</p>
          <p>Veuillez <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec  le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <section>
    <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage </h2>
    <p>Utilisez les  badges (indicateurs numériques) afin de souligner le nombre de mises à jour, d'éléments nouveaux ou non lus associés à un lien.</p>
  </section>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base </h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Valeur par défaut </h4>
  <p>Utiliser pour souligner des éléments nouveaux ou à jour avec un badge  numérique simple gris ou bleu en forme de bouton. </p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0 h5">Apparence</h5>
          <p><a href="#">Boîte de réception –  <span class="badge">42<span class="wb-inv"> courriels non lus</span></span></a></p>
          <p><a class="btn btn-primary" href="#">Boîte de réception –  <span class="badge">42<span class="wb-inv"> courriels non lus </span></span></a></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Placez <code>.badge</code> à droite du lien</li>
        <li>Assurez-vous que le  badge est dynamique, en ce sens qu'une fois que les items sont exécutés, la valeur numérique est réduite</li>
        <li>Veillez à ce qu'il ne contienne que des renseignements numériques</li>
        <li>Assurez-vous que le badge comprenne un texte invisible pour qu'il soit  descriptif.  Par exemple&nbsp;: <code>&lt;p&gt;&lt;a href=&quot;#&quot;&gt;Boîte de réception &lt;span class=&quot;badge&quot;&gt;42&lt;span class=&quot;wb-inv&quot;&gt; courriels non lus &lt;/span&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;</code></li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger h5"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>N'indiquez pas qu'il y a zéro «&nbsp;0&nbsp;» élément; s'il n'y a aucun élément, le badge devrait disparaître</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Badge gris :
&lt;p&gt;&lt;a href=&quot;#&quot;&gt;Boîte de réception &lt;span <strong>class=&quot;badge&quot;</strong>&gt;42&lt;span class=&quot;wb-inv&quot;&gt;courriels non lus &lt;/span&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;

// Badge bleu sous forme de bouton :
&lt;p&gt;&lt;a <strong>class=&quot;btn btn-primary&quot;</strong> href=&quot;#&quot;&gt;Boîte de réception &lt;span <strong>class=&quot;badge&quot;</strong>&gt;42&lt;span class=&quot;wb-inv&quot;&gt; courriels non lus&lt;/span&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Utilisation améliorée </h3>
  <h4 id="collapsing"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-times fa-stack-1x fa-inverse"></span></span> Badges qui se réduisent  seuls </h4>
  <p>Utilisez-les lorsqu'il n'y a aucun élément nouveau ou non lu. Les badges  se réduisent simplement (au moyen du <code>sélecteur empty</code> du <abbr title="feuille de style en cascade">CSS</abbr>). </p>
  <section class="alert alert-danger">
    <h4 class="mrgn-tp-0">Compatibilité multinavigateur </h4>
    <p>Les badges ne se réduiront pas seuls dans Internet Explorer 8 parce qu'il manque de soutien pour le sélecteur<code> empty</code>.</p>
  </section>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p><a href="#">Boîte de réception  <span class="badge"></span></a></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>Enlevez le contenu dans le  badge et  se réduira de lui-même, au lieu de supprimer le  badge</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation  </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Aucun contenu à l'intérieur du badge:
&lt;p&gt;&lt;a href=&quot;#&quot;&gt;... &lt;span <strong>class=&quot;badge&quot;</strong>&gt;&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires </h4>
  <p>Des ffonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="buttons-en.html">Boutons</a></li>
    <li><a class="btn btn-default" href="listgroup-en.html">Groupe de listes </a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a></p>
{% endraw %}
{:/}
