---
published: true
layout: default-theme-wet-boew-fr
title: Couleur
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
                <li><a href="#basic">Utilisation de base </a> </li>
                <li><a href="#enhanced">Utilisation améliorée </a>
                  <ul>
                    <li><a href="#addon">Fonctions complémentaires </a> </li>
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
          <p>Veuillez <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage </h2>
  <p>Utiliser la couleur comme un élément de présentation à des fins décoratives ou pour transmettre des renseignements.</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation</h3>
  <h4 id="muted"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-adjust fa-stack-1x fa-inverse"></span></span> Sourde </h4>
  <p>Utilisez pour rendre  le texte d'apparence de couleur grise   (sourde).</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-muted">Ce texte est stylisé avec  <code>.text-muted</code>.</p>
          <p>Icône colorée&nbsp;: <span class="fa fa-adjust text-muted"></span></p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez-la pour  atténuer l'apparence du texte (le rendre moins évident)</li>
        <li>Enveloppez le texte dans une balise <code>&lt;span&gt;</code> si un style n'apparaît pas comme il le devrait pour des raisons de spécificité</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Ne l'utilisez pas comme seul moyen de communiquer les renseignements ou l'intention, car la couleur seule n'est pas accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Texte de couleur sourde&nbsp;:
&lt;p <strong>class=&quot;text-muted&quot;</strong>&gt;...&lt;/p&gt;

//  Icône de couleur sourde&nbsp;:
&lt;span class=&quot;fa fa-adjust <strong>text-muted</strong>&quot;&gt;&lt;/span&gt;</code></pre>
    </div>
  </div>
  <h4 id="primary"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-tint fa-stack-1x fa-inverse"></span></span> Couleur primaire </h4>
  <p>Utilisez-la pour styliser les renseignements primaires. Les options comprennent le texte en bleu moyen, une icône bleu «&nbsp;drip&nbsp;» ou un texte blanc avec un arrière-plan bleu moyen. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-primary">Ce texte est stylisé avec  <code>.text-primary</code>.</p>
          <p>Icône colorée : <span class="fa fa-tint text-primary"></span></p>
          <p class="bg-primary">Ce texte est stylisé avec  <code>.bg-primary</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
<p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez pour faire correspondre le texte à la  palette des principales couleurs du site</li>
        <li> Enveloppez le texte dans une balise <code>&lt;span&gt;</code> si un style n'apparaît pas comme il le devrait pour des raisons de spécificité</li>
        <li>Sachez que le texte bleu peut causer des problèmes d'utilisabilité, car on peut le prendre par erreur pour un lien</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p><ul>
<li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
<li>Ne l'utilisez pas comme seul moyen de communiquer les renseignements ou l'intention, car la couleur seule n'est pas accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Texte primaire&nbsp;:
&lt;p <strong>class=&quot;text-primary&quot;</strong>&gt;...&lt;/p&gt;

// Icône primaire&nbsp;:
&lt;span class=&quot;fa fa-tint<strong> text-primary</strong>&quot;&gt;&lt;/span&gt;

// Arrière-plan primaire&nbsp;:
&lt;p <strong>class=&quot;bg-primary&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="success"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-check fa-stack-1x fa-inverse"></span></span> Couleur de succès</h4>
  <p>Utilisez-la pour styliser les renseignements de succès. Ce style comprend des options pour le texte vert, une icône représentant une coche verte ou un texte par défaut avec une arrière-plan vert pâle.  </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-success">Ce texte est stylisé avec  <code>.text-success</code>.</p>
          <p>Icône colorée&nbsp;: <span class="fa fa-check text-success"></span></p>
          <p class="bg-success">Ce texte est stylisé avec  <code>.bg-success</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez-la pour laisser entendre que le contenu est exact ou indiquer la bonne façon de faire quelque chose</li>
        <li>  Enveloppez le texte dans une balise <code>&lt;span&gt;</code> si un style n'apparaît pas comme il le devrait pour des raisons de spécificité</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p><ul>

        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li> Ne l'utilisez pas comme seul moyen de communiquer les renseignements ou l'intention, car la couleur seule n'est pas accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Texte de succès&nbsp;:
&lt;p <strong>class=&quot;text-success&quot;</strong>&gt;...&lt;/p&gt;

// Icône de succès&nbsp;:
&lt;span class=&quot;fa fa-check <strong>text-success</strong>&quot;&gt;&lt;/span&gt;

// Arrière-plan de succès&nbsp;:
&lt;p <strong>class=&quot;bg-success&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="info"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Couleur des renseignements</h4>
  <p>Utilisez-la pour styliser des renseignements relativement importants. Ce  style comprend des options pour le texte bleu, une icône représentant un «&nbsp;i&nbsp;» bleu ou un texte par défaut avec un arrière-plan bleu pâle.  </p>

  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearance</h5>
          <p class="text-info">Ce texte est stylisé avec <code>.text-info</code>.</p>
          <p>Icône colorée : <span class="fa fa-info text-info"></span></p>
          <p class="bg-info">Ce texte est stylisé avec  <code>.bg-info</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez-la pour souligner des renseignements relativement importants</li>
        <li> Enveloppez le texte dans une balise <code>&lt;span&gt;</code> si un style n'apparaît pas comme il le devrait pour des raisons de spécificité</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p><ul>
<li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
<li> Ne l'utilisez pas comme seul moyen de communiquer les renseignements ou l'intention, car la couleur seule n'est pas accessible</li>
</ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Texte de renseignements&nbsp;:
&lt;p <strong>class=&quot;text-info&quot;</strong>&gt;...&lt;/p&gt;

// Icône de renseignements&nbsp;:
&lt;span class=&quot;fa fa-info <strong>text-info</strong>&quot;&gt;&lt;/span&gt;

// Arrière-plan de renseignements&nbsp;:
&lt;p <strong>class=&quot;bg-info&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="warning"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-triangle fa-stack-1x fa-inverse"></span></span> Couleur d'avertissement</h4>
  <p>Utilisez-la pour styliser les renseignements d'avertissement. Ce  style comprend des options pour le texte brun, une icône représentant un point d'exclamation dans un triangle ou un texte par défaut avec un arrière-plan brun doré pâle. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-warning">Ce texte est stylisé avec  <code>.text-warning</code>.</p>
          <p>Icône colorée : <span class="fa fa-exclamation-triangle text-warning"></span></p>
          <p class="bg-warning">Ce texte est stylisé avec <code>.bg-warning</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez-la pour attirer l'attention sur le contenu et avertir l'utilisateur de quelque chose</li>
        <li> Enveloppez le texte dans une balise <code>&lt;span&gt;</code> si un style n'apparaît pas comme il le devrait pour des raisons de spécificité</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
<li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
<li> Ne l'utilisez pas comme seul moyen de communiquer les renseignements ou l'intention, car la couleur seule n'est pas accessible</li>
</ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Texte d'avertissement&nbsp;:
&lt;p <strong>class=&quot;text-warning&quot;</strong>&gt;...&lt;/p&gt;

// Icône d'avertissement&nbsp;:
&lt;span class=&quot;fa fa-exclamation-triangle <strong>text-warning</strong>&quot;&gt;&lt;/span&gt;

// Arrière-plan d'avertissement&nbsp;:
&lt;p <strong>class=&quot;bg-warning&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="danger"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-circle fa-stack-1x fa-inverse"></span></span> Couleur de danger </h4>
  <p>Utilisez-la pour styliser des renseignements très importants. Ce style comprend des options pour un texte rouge, une icône représentant une point d'exclamation dans un cercle ou le texte par défaut avec un arrière-plan rouge pâle.  </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-danger">Ce texte est stylisé avec  <code>.text-danger</code>.</p>
          <p>Icône colorée : <span class="fa fa-exclamation-circle text-danger"></span></p>
          <p class="bg-danger">Ce texte est stylisé avec  <code>.bg-danger</code>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Utilisez-la pour attirer l'attention sur un contenu très important et aviser l'utilisateur qu'une action est dangereuse</li>
        <li> Enveloppez le texte dans une balise <code>&lt;span&gt;</code> si un style n'apparaît pas comme il le devrait pour des raisons de spécificité</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>

        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>  Ne l'utilisez pas comme seul moyen de communiquer les renseignements ou l'intention, car la couleur seule n'est pas accessible</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Texte de danger&nbsp;:
&lt;p <strong>class=&quot;text-danger&quot;</strong>&gt;...&lt;/p&gt;


// Icône de danger&nbsp;:
&lt;span class=&quot;fa fa-exclamation-circle <strong>text-danger</strong>&quot;&gt;&lt;/span&gt;

// Arrière-plan de danger&nbsp;:
&lt;p <strong>class=&quot;bg-danger&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Utilisation améliorée </h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires </h4>
  <p>Des fonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="icons-en.html">Icônes</a></li>
  </ul>

  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Principes de soutien</h2>
  <div data-ajax-replace="../writing/strctr-fr.html #colour-info"></div>

    <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a></p>
{% endraw %}
{:/}
