---
published: true
layout: default-theme-wet-boew-fr
title: Pagination
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
                <li><a href="#enhanced">Utilisation améliorée</a>
                  <ul>
                    <li> <a href="#active">État actif </a></li>
                    <li><a href="#disabled">État désactivé </a></li>
                    <li><a href="#sizing">Redimensionnement</a></li>
                    <li><a href="#pager">SimplePager </a></li>
                    <li><a href="#addon">Fonctions complémentaires</a> </li>
                  </ul>
                </li>
              </ul>
            </li>
            <li><a href="#supporting">Principes à l'appui</a></li>
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
  <p>Utilisez un index de pagination pour les documents longs qu'il est préférable de diviser en plusieurs pages. Un utilisateur peut sélectionner une page particulière dans un document à l'aide des fonctions « Suivant » ou « Précédent », ou (s'ils sont présents) des hyperliens de pagination numériques.</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Défaut</h4>
  <p>L'utiliser pour séparer des éléments de contenu et les étendre sur un grand nombre de pages. Ainsi, les sections au contenu volumineux sont plus faciles à lire.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <ul class="pagination">
            <li><a href="#" rel="prev">Précédent</a></li>
            <li><a href="#">1 <span class="wb-inv">Aller à la page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Aller à la page 2</span></a></li>
            <li><a href="#" rel="next">Suivant</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.pagination</code> pour numéroter les pages distinctes d'une section au contenu volumineux</li>
        <li>Assurez-vous que la pagination est toujours alignée à gauche</li>
        <li>Assurez-vous que les liens de navigation s'affichent sur une seule rangée et <strong>n'activez pas le retour à la ligne</strong>, à moins qu'il y ait une raison valide de le faire</li>
        <li>Ajoutez du texte invisible à l'aide de  <code>&lt;span class"wb-inv"&gt;</code> pour rendre les liens descriptifs</li>
        <li>Assurez-vous qu'il y a un espace entre le numéro de pagination et <code>&lt;span class"wb-inv"&gt;</code> pour faire en sorte que les lecteurs d'écran puissent interpréter correctement le code</li>
        <li>Comprenez et mettez en œuvre les <a href="#supporting"> principes à l'appui</a> connexes</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;ul <strong>class=&quot;pagination&quot;</strong>&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; <strong>rel=&quot;prev&quot;</strong>&gt;Précédent&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot;&gt;1 <strong>&lt;span class=&quot;wb-inv&quot;&gt;Aller à la page  </strong> 1&lt;/span&gt;&lt;/a&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot;&gt;2 <strong>&lt;span class=&quot;wb-inv&quot;&gt;Aller à la page  </strong> 2&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; <strong>rel=&quot;next&quot;</strong>&gt;Suivant&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Utilisation améliorée</h3>
  <h4 id="active"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-bolt fa-stack-1x fa-inverse"></span></span> État actif </h4>
  <p> L'utiliser pour indiquer la page actuelle où se trouve l'utilisateur.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <ul class="pagination">
            <li><a href="#" rel="prev">Précédent</a></li>
            <li class="active"><a href="#">1 <span class="wb-inv">(cette page) Aller à la page  1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Aller à la page 2</span></a></li>
            <li><a href="#" rel="next">Suivant</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.active</code> pour indiquer la page actuelle où se trouve l'utilisateur dans la pagination</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;ul class=&quot;pagination&quot;&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Précédent&lt;/a&gt;&lt;/li&gt;
  &lt;li <strong>class=&quot;active&quot;</strong>&gt;&lt;a href=&quot;#&quot;&gt;1 &lt;span class=&quot;wb-inv&quot;&gt;<strong>(current)</strong> Aller à la page  1&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
  ...
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="disabled"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> État désactivé</h4>
  <p> L'utiliser pour cacher des éléments de navigation inutiles, par exemple, un bouton « Précédent » si l'utilisateur se trouve à la « page 1 » d'une section de contenu.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>« Précédent » est désactivé, est donc caché :</p>
          <ul class="pagination">
            <li class="disabled"><a href="#" rel="prev">Précédent</a></li>
            <li><a href="#">1 <span class="wb-inv">Aller à la page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Aller à la page 2</span></a></li>
            <li><a href="#" rel="next">Suivant</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li> Utilisez <code>.disabled</code> pour les liens non cliquables (cachés) à l'intérieur de la pagination</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;ul class=&quot;pagination&quot;&gt;
  &lt;li <strong>class=&quot;disabled&quot;</strong>&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Précédent&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot;&gt;1 &lt;span class=&quot;wb-inv&quot;&gt;Aller à la page  1&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
  ...
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="sizing"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-expand fa-stack-1x fa-inverse"></span></span> Redimensionnement</h4>
  <p>Utilisez <code>.pagination-lg</code> ou <code>.pagination-sm</code> pour les options de taille de pagination supplémentaires.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Défaut :</p>
          <ul class="pagination mrgn-tp-0 mrgn-bttm-md">
            <li><a href="#" rel="prev">Précédent</a></li>
            <li><a href="#">1 <span class="wb-inv">Aller à la page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Aller à la page 2</span></a></li>
            <li><a href="#" rel="next">Suivant</a></li>
          </ul>
          <p>Grand :</p>
          <ul class="pagination pagination-lg mrgn-tp-0 mrgn-bttm-md">
            <li><a href="#" rel="prev">Précédent</a></li>
            <li><a href="#">1 <span class="wb-inv">Aller à la page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Aller à la page 2</span></a></li>
            <li><a href="#" rel="next">Suivant</a></li>
          </ul>
          <p>Petit :</p>
          <ul class="pagination pagination-sm mrgn-tp-0 mrgn-bttm-0">
            <li><a href="#" rel="prev">Précédent</a></li>
            <li><a href="#">1 <span class="wb-inv">Aller à la page 1</span></a></li>
            <li><a href="#">2 <span class="wb-inv">Aller à la page 2</span></a></li>
            <li><a href="#" rel="next">Suivant</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li><strong>Taille par défaut :</strong> L'utiliser pour une pagination typique</li>
        <li><strong>Petits boutons :</strong> Les utiliser lorsque la pagination apparaît dans un petit espace. Cela permet de réduire la taille des boutons afin de maximiser le nombre de boutons qui s'affichent dans une seule rangée</li>
        <li><strong>Gros bouton :</strong> L'utiliser lorsque la pagination doit être plus évidente sur la page. Puisque les boutons par défaut assurent déjà une mise en évidence et un appel à l'action, l'augmentation de la taille de ces boutons est peu utile ou nécessaire</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Défaut :
&lt;ul class=&quot;pagination&quot;&gt;...&lt;/ul&gt;

// Grand :
&lt;ul class=&quot;pagination <strong>pagination-lg</strong>&quot;&gt;...&lt;/ul&gt;

// Petit :
&lt;ul class=&quot;pagination <strong>pagination-sm</strong>&quot;&gt;...&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="pager"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8644;</span></span> SimplePager</h4>
  <p>L'utiliser pour créer une pagination simple de liens « Précédent » et « Suivant » seulement.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Défaut</p>
          <ul class="pager">
            <li><a href="#" rel="prev">Précédent</a></li>
            <li><a href="#" rel="next">Suivant</a></li>
          </ul>
          <p>Boutons de justification complète</p>
          <ul class="pager">
            <li class="previous"><a href="#" rel="prev">Précédent</a></li>
            <li class="next"><a href="#" rel="next">Suivant</a></li>
          </ul>
          <p>État désactivé (bouton « Précédent » caché) </p>
          <ul class="pager">
            <li class="previous disabled"><a href="#" rel="prev">Précédent</a></li>
            <li class="next"><a href="#" rel="next">Suivant</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.pager</code> lorsqu'il faut <strong>seulement </strong>établir un lien avec la page « Précédent » ou « Suivant »</li>
        <li>Utilisez <code>.previous</code> et <code>.next</code> à l'intérieur des éléments <code>&lt;li&gt;</code> pour justifier entièrement les liens  <code>&lt;ul class=&quot;pager&quot;</code></li>
        <li>Comprenez et mettez en œuvre les <a href="#supporting"> principes à l'appui</a> connexes</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Défaut :
&lt;ul <strong>class=&quot;pager&quot;</strong>&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Précédent&lt;/a&gt;&lt;/li&gt;
  &lt;li&gt;&lt;a href=&quot;#&quot; rel=&quot;next&quot;&gt;Suivant&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;

// Boutons de justification complète :
&lt;ul class=&quot;pager&quot;&gt;
  &lt;li <strong>class=&quot;previous&quot;</strong>&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Précédent&lt;/a&gt;&lt;/li&gt;
  &lt;li <strong>class=&quot;next&quot;</strong>&gt;&lt;a href=&quot;#&quot; rel=&quot;next&quot;&gt;Suivant&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;

// État désactivé (« Précédent » caché) :
&lt;ul class=&quot;pager&quot;&gt;
  &lt;li class=&quot;previous <strong>disabled</strong>&quot;&gt;&lt;a href=&quot;#&quot; rel=&quot;prev&quot;&gt;Précédent&lt;/a&gt;&lt;/li&gt;
  &lt;li class=&quot;next&quot;&gt;&lt;a href=&quot;#&quot; rel=&quot;next&quot;&gt;Suivant&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires</h4>
  <p>Des caractéristiques et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="buttons-fr.html">Boutons</a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Principes à l'appui</h2>
  <h3><span data-ajax-replace="../writing/rchtctr-fr.html #length-heading"></span></h3>
  <div data-ajax-replace="../writing/rchtctr-fr.html #length-info"></div>
  <h3><span data-ajax-replace="../writing/stl-fr.html #scent-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-fr.html #scent-info"></div>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a></p>
{% endraw %}
{:/}
