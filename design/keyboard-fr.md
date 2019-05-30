---
published: true
layout: default-theme-wet-boew-fr
title: Touches de clavier
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
                <li><a href="#basic">Utilisation de base</a></li>
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
          <p>Veuillez  <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <section>
    <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage</h2>
    <p>Utiliser pour reproduire les touches d'un clavier d'ordinateur. </p>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
    <h3 id="basic">Utilisation de base</h3>
	 <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Défaut</h4>
     <p>Utilisez pour présenter des touches de clavier.</p>
     <div class="row">
      <div class="col-md-4">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Apparence</h5>
            <p>Appuyez sur <kbd>Shift</kbd></p>
            <p>Appuyez sur <kbd><abbr title="Contrôle">Ctrl</abbr></kbd></p>
            <p>Appuyez sur <kbd>Enter</kbd></p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
<p>Points de conformité&nbsp;:</p>
        <ul>
          <li>Utilisez <code>&lt;kbd&gt;</code> pour décrire une touche de clavier qu'un utilisateur doit sélectionner dans un processus</li>
              <li>Utilisez l'orthographe, l'espacement et la casse de phrase appropriés du texte de clavier, par exemple , <kbd><abbr title="Contrôle">Ctrl</abbr></kbd>)</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
        <p>Points de conformité&nbsp;:</p><ul>
          <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
          <li>Ne l'utilisez pas pour le nom de menus ou le texte de contenu</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>&lt;p&gt;Appuyez sur <strong>&lt;kbd&gt;</strong>Shift<strong>&lt;/kbd&gt;</strong>&lt;/p&gt;
&lt;p&gt;Appuyez sur &lt;kbd&gt;&lt;abbr title=&quot;Contrôle&quot;&gt;Ctrl&lt;/abbr&gt;&lt;/kbd&gt;&lt;/p&gt;
&lt;p&gt;Appuyez sur &lt;kbd&gt;Entrée&lt;/kbd&gt;&lt;/p&gt;</code></pre>
      </div>
    </div>
  </section>
  <p class="mrgn-tp-lg text-muted"> Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" rel="external">Bootstrap<span class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
