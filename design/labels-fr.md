---
published: true
layout: default-theme-wet-boew-fr
title: Étiquettes
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
            <li><a href="#design">Conception et codage</a>
              <ul>
                <li><a href="#basic">Utilisation de base </a>
                  <ul>
                    <li><a href="#default">Étiquette par défaut </a></li>
                    <li><a href="#primary">Étiquette primaire</a></li>
                    <li><a href="#success">Étiquette de succès</a></li>
                    <li><a href="#info">Étiquette d'information</a></li>
                    <li><a href="#warning">Étiquette d'avertissement</a></li>
                    <li><a href="#danger">Étiquette de danger</a></li>
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
          <h2 class="mrgn-tp-0 h4 text-warning"><span class="fa fa-exclamation-triangle"></span>Chantier</h2>
          <p>Cette page est en chantier.</p>
          <p>Veuillez <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage si des renseignements ou des codes son manquants, incorrects ou que leur synchronisation est déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage </h2>
  <p>Utiliser l'étiquette appropriée pour décrire et mettre en surbrillance des renseignements textuels (non numériques).</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Étiquette par défaut</h4>
  <p>Utilisez-la pour présenter quelques mots à l'arrière-plan. Elle donne du contexte supplémentaire sur le contenu adjacent.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Du texte ici  <span class="label label-default">(Information sur l'étiquette)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p>Point d'observation&nbsp;:</p>
      <ul>
        <li>Utilisez <code>.label-default</code> pour attirer l'attention sur une section de contenu en ajoutant de courts éléments de renseignements textuels à l'appui</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
        <li>Ne l'utilisez pas dans les alertes ou les boutons</li>
        <li>Ne l'utilisez pas pour mettre en surbrillance des éléments non lus − utilisez des <a href="badges-fr.html">badges</a></li>
        <li>Ne mettez pas en surbrillance des grandes sections de texte − utilisez des <a href="alerts-fr.html">alertes</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Du texte ici <strong>&lt;span class=&quot;label label-default&quot;&gt;</strong>(Information sur l'étiquette)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="primary"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-certificate fa-stack-1x fa-inverse"></span></span> Étiquette primaire </h4>
  <p>Utilisez-la pour présenter quelques mots sur un arrière-plan coloré  qui correspond au thème de couleur du  site. Elle donne un contexte supplémentaire sur le contenu adjacent.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Du texte ici <span class="label label-primary">(Information sur l'étiquette)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>Utilisez <code>.label-primary</code> pour attirer l'attention sur une section de contenu en ajoutant de courts éléments de renseignements textuels à l'appui</li>
        <li>Utilisez pour faire correspondre l'étiquette au thème de couleur du site</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Ne l'utilisez pas dans les alertes ou les boutons</li>
        <li>Ne l'utilisez pas pour mettre en surbrillance des éléments non lus − utilisez des <a href="badges-fr.html">badges</a></li>
        <li>Ne mettez pas en surbrillance de grandes sections de texte − utilisez des <a href="alerts-fr.html">alertes</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Du texte ici <strong>&lt;span class=&quot;label label-primary&quot;&gt;</strong>(Information sur l'étiquette)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="success"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-check fa-stack-1x fa-inverse"></span></span> Étiquette de succès</h4>
  <p>Utilisez-la pour présenter quelques mots sur un arrière-plan coloré qui laissent entendre que le contenu est exact. Elle donne un contexte supplémentaire sur le contenu adjacent.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-success">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Du texte ici <span class="label label-success">(Information sur l'étiquette)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>Utilisez <code>.label-success</code> pour attirer l'attention sur une section de contenu en ajoutant de courts éléments de renseignements textuels à l'appui</li>
        <li>Utilisez-la pour indiquer que le contenu est exact</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Ne l'utilisez pas dans les alertes ou les boutons</li>
        <li>Ne l'utilisez pas pour mettre en surbrillance des éléments non lus − utilisez des <a href="badges-fr.html">badges</a></li>
        <li>Ne mettez pas en surbrillance de grandes sections de texte − utilisez des <a href="alerts-fr.html">alertes</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Du texte ici <strong>&lt;span class=&quot;label label-success&quot;&gt;</strong>(Information sur l'étiquette)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="info"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Étiquette de renseignements </h4>
  <p>Utilisez-la pour présenter quelques mots sur un arrière-plan coloré qui laissent entendre que le contenu est informatif. Elle donne un contexte supplémentaire sur le contenu adjacent.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Du texte ici <span class="label label-info">(Information sur l'étiquette)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>Utilisez-la pour indiquer que l'utilisateur doit être averti</li>
        <li>Utilisez <code>.label-info</code> pour attirer l'attention sur une section de contenu en ajoutant de petits éléments textuels de renseignements à l'appui</li>
        <li>Utilisez-la pour indiquer que le contenu est de nature informative</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Ne l'utilisez pas dans les alertes ou les boutons</li>
        <li>Ne l'utilisez pas pour mettre en surbrillance des éléments non lus − utilisez des <a href="badges-fr.html">badges</a></li>
        <li>Ne mettez pas en surbrillance de grandes sections de texte − utilisez des <a href="alerts-fr.html">alertes</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Du texte ici <strong>&lt;span class=&quot;label label-info&quot;&gt;</strong>(Information sur l'étiquette)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="warning"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-triangle fa-stack-1x fa-inverse"></span></span> Étiquette d'avertissement</h4>
  <p>Utilisez-la pour présenter quelques mots sur un arrière-plan coloré qui laissent entendre que l'utilisateur doit être averti. Elle donne un contexte supplémentaire sur le contenu adjacent.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Du texte ici <span class="label label-warning">(Information sur l'étiquette)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>Utilisez <code>.label-warning</code> pour attirer l'attention sur une section de contenu en ajoutant de courts éléments de renseignements textuels à l'appui</li>
        <li>Utilisez pour indiquer que l'utilisateur doit être averti</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Ne l'utilisez pas dans les alertes ou les boutons</li>
        <li>Ne l'utilisez pas pour mettre en surbrillance des éléments non lus − utilisez des <a href="badges-fr.html">badges</a></li>
        <li>Ne mettez pas en surbrillance de grandes sections de texte − utilisez des <a href="alerts-fr.html">alertes</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Du texte ici <strong>&lt;span class=&quot;label label-warning&quot;&gt;</strong>(Information sur l'étiquette)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <h4 id="danger"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-circle fa-stack-1x fa-inverse"></span></span> Étiquette de danger </h4>
  <p>Utilisez-la pour présenter quelques mots sur un arrière-plan coloré qui laissent entendre que l'action ou le contenu est dangereux. Elle donne un contexte supplémentaire sur le contenu adjacent.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Du texte ici <span class="label label-danger">(Information sur l'étiquette)</span></p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>Utilisez <code>.label-danger</code> pour attirer l'attention sur une section de contenu en ajoutant de courts éléments de renseignements textuels à l'appui</li>
        <li>Utilisez-la pour indiquer que l'action ou le contenu est dangereux</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Ne l'utilisez pas dans les alertes ou les boutons</li>
        <li>Ne l'utilisez pas pour mettre en surbrillance des éléments non lus − utilisez des  <a href="badges-fr.html">badges</a></li>
        <li>Ne mettez pas en surbrillance de grandes sections de texte − utilisez des <a href="alerts-fr.html">alertes</a></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;Du texte ici <strong>&lt;span class=&quot;label label-danger&quot;&gt;</strong>(Information sur l'étiquette)&lt;/span&gt;&lt;/p&gt;
	  </code></pre>
    </div>
  </div>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" rel="external">Bootstrap<span class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
