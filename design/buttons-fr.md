---
published: true
layout: default-theme-wet-boew-fr
title: Boutons
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
                    <li><a href="#colour">Couleurs</a></li>
                    <li><a href="#sizing">Taille</a></li>
                    <li><a href="#buttons-block">Largeur maximale </a></li>
                    <li><a href="#buttons-active">État d'activation</a></li>
                    <li><a href="#buttons-disabled">État de désactivation </a></li>
                    <li><a href="#btn-groups">Groupes</a></li>
                    <li><a href="#btn-toolbars">Barres à outils </a></li>
                    <li><a href="#btn-types">Genres de boutons</a></li>
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
          <p>Cette page porte sur le travail en cours.</p>
          <p>Veuillez   <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage</h2>
  <p>Utilisez des boutons pour créer un appel à l'action qui incite l'utilisateur à soumettre du contenu à partir d'un formulaire. De plus, utilisez des boutons pour amener les utilisateurs à une page Web qui présente des renseignements supplémentaires. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Par défaut </h4>
  <p>Utilisez les catégories de boutons sur des éléments <code>&lt;a&gt;</code>, <code>&lt;button&gt;</code> ou <code>&lt;input&gt;</code> afin de créer une uniformité visuelle. Le navigateur présente certains éléments comme un bouton. Toutefois, il manque d'uniformité visuelle pour chaque genre de bouton. L'apparence de bouton par défaut peut être différente pour chaque navigateur.</p>

  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="row">
            <div class="col-sm-6">
              <h6>Par défaut</h6>
              <ul class="list-unstyled lst-spcd">
                <li>
                  <button type="submit">Bouton</button>
                </li>
                <li>
                  <input type="button" value="Entrer" />
                </li>
                <li>
                  <input type="submit" value="Soumettre" />
                </li>
                <li><a href="#">Lien</a></li>
              </ul>
            </div>
            <div class="col-sm-6">
              <h6>Stylisé </h6>
              <ul class="list-unstyled lst-spcd">
                <li>
                  <button class="btn btn-default" type="submit">Bouton</button>
                </li>
                <li>
                  <input class="btn btn-default" type="button" value="Saisir" />
                </li>
                <li>
                  <input class="btn btn-default" type="submit" value="Soumettre" />
                </li>
                <li><a class="btn btn-default" href="#" role="button">Lien</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li><strong>Utilisez l'élément  <code>&lt;button&gt;</code> tant que possible</strong> afin de vous assurer  de la concordance avec le rendu multinavigateur
              <ul>
            <li>Il y a un<a href="https://bugzilla.mozilla.org/show_bug.cgi?id=697451" > bogue dans  Firefox &lt;30</a> that qui rend impossible l'établissement de  <code>line-height</code> dans les boutons fondés sur <code>&lt;input&gt;</code></li>
            <li>La hauteur de ces boutons est inégale dans Firefox</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
     </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>


    <pre><code>// Bouton par défaut&nbsp;:
&lt;button type=&quot;submit&quot;&gt;Bouton&lt;/button&gt;
&lt;input type=&quot;button&quot; <strong>value=&quot;Saisir&quot;</strong> /&gt;
&lt;input type=&quot;submit&quot; <strong>value=&quot;Soumettre&quot;</strong> /&gt;
<strong>&lt;a class=&quot;btn btn-default&quot;</strong> href=&quot;#&quot;&lt;/a&gt;

// Bouton stylisé :
<strong>&lt;button class=&quot;btn btn-default&quot; type=&quot;submit&quot;</strong>&gt;Button&lt;/button&gt;
&lt;input class=&quot;btn btn-default&quot; type=&quot;button&quot;<strong> value=&quot;Saisir&quot;</strong> /&gt;
&lt;input class=&quot;btn btn-default&quot; type=&quot;submit&quot; <strong>value=&quot;Soumettre&quot;</strong> /&gt;
&lt;a <strong>class=&quot;btn btn-default&quot;</strong> href=&quot;#&quot; <strong>role=&quot;button&quot;</strong>&gt;Lien&lt;/a&gt;</code></pre>
  </div>
   </div>
  <h3 id="enhanced">Utilisation améliorée </h3>
  <h4 id="colour"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-tint fa-stack-1x fa-inverse"></span></span> Couleurs</h4>
  <p>Utilisez pour ajouter des couleurs aux boutons. Les couleurs signifient notamment un lien vers des renseignements d'avertissement (bouton d'avertissement) à un lien vers le prochain module d'apprentissage (bouton succès).</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <ul class="list-unstyled lst-spcd">
            <li>
              <button type="button" class="btn btn-default">Par défaut</button>
            </li>
            <li>
              <button type="button" class="btn btn-primary">Primaire</button>
            </li>
            <li>
              <button type="button" class="btn btn-success">Succès</button>
            </li>
            <li>
              <button type="button" class="btn btn-info">Info</button>
            </li>
            <li>
              <button type="button" class="btn btn-warning">Avertissement</button>
            </li>
            <li>
              <button type="button" class="btn btn-danger">Danger</button>
            </li>
            <li>
              <button type="button" class="btn btn-link">Lien</button>
            </li>
          </ul>
        </div>
      </div>
    </div>

    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez les boutons comme suit :
          <ul>
            <li><strong>Par défaut&nbsp;:</strong> Bouton standard </li>
            <li><strong>Primaire :</strong> Donne un poids visuel supplémentaire et indique l'action primaire dans un ensemble de boutons</li>
            <li><strong>Succès :</strong> Indique une action réussie ou positive qui permet à l'utilisateur de passer à phase suivante ou au module suivant</li>
            <li><strong>Info :</strong> Bouton contextuel pour les messages d'alerte informationnels</li>
            <li><strong>Avertissement :</strong> Indique que la prudence sera de mise avec cette  action</li>
            <li><strong>Danger :</strong> Indique une action dangereuse ou potentiellement négative</li>
            <li><strong>Lien :</strong> Réduit le rôle du bouton en le faisant ressembler à un lien, tout en maintenant le comportement d'un bouton</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Défaut&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn <strong>btn-default&quot;</strong>&gt;Défaut&lt;/button&gt;

// Primaire :
&lt;button type=&quot;button&quot; class=&quot;btn <strong>btn-primary&quot;</strong>&gt;Primaire&lt;/button&gt;

// Succès&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn <strong>btn-success&quot;</strong>&gt;Succès&lt;/button&gt;

// Info&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn <strong>btn-info&quot;</strong>&gt;Info&lt;/button&gt;

// Avertissement&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn <strong>btn-warning&quot;</strong>&gt;Avertissement&lt;/button&gt;

// Danger&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn <strong>btn-danger&quot;</strong>&gt;Danger&lt;/button&gt;

// Lien&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn <strong>btn-link&quot;</strong>&gt;Lien&lt;/button&gt;</code></pre>
    </div>
  </div>
  <h4 id="sizing"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-expand fa-stack-1x fa-inverse"></span></span> Taille </h4>
  <p>Utilisez pour augmenter ou diminuer la taille d'un bouton.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <ul class="list-unstyled lst-spcd">
            <li>
              <button type="button" class="btn btn-default btn-lg">Gros bouton</button>
            </li>
            <li>
              <button type="button" class="btn btn-default">Bouton par défaut </button>
            </li>
            <li>
              <button type="button" class="btn btn-default btn-sm">Petit bouton</button>
            </li>
            <li>
              <button type="button" class="btn btn-default btn-xs">Très petit bouton </button>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li><strong>Taille par défaut :</strong> Utilisez pour un bouton ordinaire</li>
        <li><strong>Boutons petits ou très petits :</strong> Utilisez lorsque plusieurs boutons se trouvent dans une barre à outils et que l'espace est restreint. La taille du bouton est réduite afin de maximiser le nombre de boutons qui figure sur une seule rangée</li>
        <li><strong>Gros bouton : </strong>Utilisez-le lorsque vous voulez lui donner une importance accrue  sur la page. Puisque les boutons par défaut crée déjà une importance et un appel à l'action,    la valeur ou le besoin d'augmenter leur taille est limité</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Gros bouton&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn btn-default <strong>btn-lg&quot;</strong>&gt;Gros bouton&lt;/button&gt;

// Bouton par défaut&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn btn-<strong>default&quot;</strong>&gt;Défaut bouton&lt;/button&gt;

// Petit bouton&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn btn-default <strong>btn-sm&quot;</strong>&gt;Petit bouton&lt;/button&gt;

// Très petit bouton&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn btn-default <strong>btn-xs&quot;</strong>&gt;Très petit bouton&lt;/button&gt;</code></pre>
    </div>
  </div>
  <h4 id="buttons-block"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-h fa-stack-1x fa-inverse"></span></span> Largeur maximale </h4>
  <p>Utilisez pour créer des boutons de blocage de niveau (ceux qui s'étend sur toute la largeur d'un contenant apparenté).</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <button type="button" class="btn btn-default btn-block">Bouton de blocage de niveau </button>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.btn-block</code> lorsque le bouton se trouve dans un petit contenant
              <ul>
            <li>Ce bouton s'étend sur toute la largeur d'un contenant apparenté et est totalement justifié dans l'espace disponible</li>
          </ul>
        </li>
        <li>Testez le bouton dans toutes les résolutions
          <ul>
            <li>Dans une conception  adaptative, les boutons qui prennent la largeur maximale peuvent ne pas avoir une belle apparence dans toutes les résolutions</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Bouton de blocage de niveau&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn btn-default <strong>btn-block&quot;</strong>&gt;Bouton de blocage de niveau&lt;/button&gt;
</code></pre>
    </div>
  </div>
  <h4 id="buttons-active"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-bolt fa-stack-1x fa-inverse"></span></span> État d'activation </h4>
  <p>Utilisez <code>.active</code> avec les éléments <code>&lt;button&gt;</code> et <code>&lt;a&gt;</code> si vous avez besoin qu'un bouton semble actif en tout temps (habituellement aux fins d'affichage et d'enseignement sur des boutons ou  liens factices). Lorsqu'un utilisateur appuie sur un bouton, il semble être actif (avec une  ombre interne, ainsi qu'un arrière-plan et une bordure plus foncés). Pour les éléments <code>&lt;button&gt;</code> et <code>&lt;a&gt;</code>, ils sont stylisés automatiquement dans <abbr title="feuille de style en cascade">CSS</abbr> au moyen de <code>:active</code>. </p>
  <p>&nbsp;</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <ul class="list-unstyled lst-spcd">
            <li>
              <button type="button" class="btn btn-default active">Bouton</button>
            </li>
            <li><a href="#" class="btn btn-default active" role="button">Lien</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Ajoutez <code>.active</code> à l'élément <code>&lt;a&gt;</code> ou <code>&lt;button&gt;</code> pour indiquer qu'un lien ou un bouton est actif</li>
        <li>Utilisez lorsque la cible de lien ou de bouton correspond à l'adresse de la page courante</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Bouton actif&nbsp;:
&lt;button type=&quot;button&quot; class=&quot;btn btn-default <strong>active</strong>&quot;&gt;Bouton&lt;/button&gt;

// Lien actif&nbsp;:
&lt;a href=&quot;#&quot; class=&quot;btn btn-default <strong>active</strong>&quot; role=&quot;button&quot;&gt;Lien&lt;/a&gt;</code></pre>
    </div>
  </div>
  <h4 id="buttons-disabled"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> État de désactivation </h4>
  <p>Utilisez pour désactiver des boutons et des liens (non cliquable) et donne une apparence décolorée.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <ul class="list-unstyled lst-spcd">
            <li>
              <button type="button" class="btn btn-default" disabled="disabled">Bouton</button>
            </li>
            <li><a href="#" class="btn btn-default disabled" role="button">Lien</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez  <code>disabled="disabled"</code> pour déactiver un bouton</li>
        <li>Ajoutez la catégorie <code>.disabled</code> à un élément <code>&lt;a&gt;</code> afin d'indiquer qu'un lien est désactivé</li>
        <li>Retirez l'attribut <code>href</code> afin de désactiver complètement les liens, car la catégorie ne change que l'apparence de la balise  <code>&lt;a&gt;</code>, non la fonctionnalité</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Bouton désactivé :
&lt;button type=&quot;button&quot; class=&quot;btn btn-default btn-lg&quot; <strong>disabled=&quot;disabled&quot;</strong>&gt;Bouton&lt;/button&gt;

// Lien désactivé&nbsp;:
&lt;a href=&quot;#&quot; class=&quot;btn btn-default btn-lg <strong>disabled</strong>&quot; role=&quot;button&quot;&gt;Lien&lt;/a&gt;</code></pre>
    </div>
  </div>
  <h4 id="btn-groups"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ellipsis-h fa-stack-1x fa-inverse"></span></span> Groupes</h4>
  <p>Utilisez pour regrouper une série de boutons sur une seule ligne avec le groupe de boutons.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Appearence</h5>
          <p>Par défaut&nbsp;:</p>
          <div class="btn-group mrgn-bttm-lg">
            <button type="button" class="btn btn-default">Gauche</button>
            <button type="button" class="btn btn-default">Centré</button>
            <button type="button" class="btn btn-default">Droite</button>
          </div>
          <p>Gros&nbsp;:</p>
          <div class="btn-group btn-group-lg mrgn-bttm-lg">
            <button type="button" class="btn btn-default">Gauche</button>
            <button type="button" class="btn btn-default">Centré</button>
            <button type="button" class="btn btn-default">Droite</button>
          </div>
          <p>Petit&nbsp;:</p>
          <div class="btn-group btn-group-sm mrgn-bttm-lg">
            <button type="button" class="btn btn-default">Gauche</button>
            <button type="button" class="btn btn-default">Centré</button>
            <button type="button" class="btn btn-default">Droite</button>
          </div>
          <p>Très petit&nbsp;:</p>
          <div class="btn-group btn-group-xs mrgn-bttm-lg">
            <button type="button" class="btn btn-default">Gauche</button>
            <button type="button" class="btn btn-default">Centré</button>
            <button type="button" class="btn btn-default">Droite</button>
          </div>
          <p>Justifié (lien)&nbsp;:</p>
          <div class="btn-group btn-group-justified mrgn-bttm-lg"> <a class="btn btn-default" role="button">Gauche</a> <a class="btn btn-default" role="button">Centré</a> <a class="btn btn-default" role="button">Droite</a> </div>
          <p>Justifié (boutons)&nbsp;:</p>
          <div class="btn-group btn-group-justified">
            <div class="btn-group">
              <button type="button" class="btn btn-default">Gauche</button>
            </div>
            <div class="btn-group">
              <button type="button" class="btn btn-default">Centré</button>
            </div>
            <div class="btn-group">
              <button type="button" class="btn btn-default">Droite</button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez pour créer une seule barre à outils de boutons</li>
        <li>Enveloppez une série de boutons avec <code>.btn</code> dans <code>.btn-group</code></li>
        <li>Ajoutez  <code>.btn-group-*</code>à <code>.btn-group</code> au lieu d'appliquer des catégories de tailles de bouton à chaque bouton d'un groupe</li>
        <li>Enveloppez une série de boutons avec <code>.btn</code> dans <code>.btn-group btn-group-justified </code> − pour utiliser des groupes de boutons justifiés avec des éléments <code>&lt;a&gt;</code></li>
        <li>Enveloppez chaque bouton dans un groupe de boutons pour utiliser des groupes de boutons justificatifs avec des éléments  <code>&lt;button&gt;</code>. La plupart des navigateurs n'appliquent notre <abbr title="feuille de style en cascade">CSS</abbr> que pour la justification aux éléments <code>&lt;button&gt;</code>. Puisque nous prenons en charge les boutons de déroulement, nous pouvons le contourner</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Par défaut&nbsp;:
&lt;div<strong> class=&quot;btn-group&quot;</strong>&gt;
  <strong>&lt;button class=&quot;btn</strong> btn-default&quot; type=&quot;button&quot;&gt;...&lt;/button&gt;...
&lt;/div&gt;

// Groupe de gros boutons :
&lt;div class=&quot;btn-group<strong> btn-group-lg&quot;</strong>&gt;...
&lt;/div&gt;

//Groupe de petits boutons&nbsp;:
&lt;div class=&quot;btn-group <strong>btn-group-sm&quot;</strong>&gt;...
&lt;/div&gt;

// Groupe de très petits boutons&nbsp;:
&lt;div class=&quot;btn-group<strong> btn-group-xs&quot;</strong>&gt;...
&lt;/div&gt;

// Liens justifiés&nbsp;:
&lt;div <strong>class="btn-group btn-group-justified"</strong>&gt;
   &lt;a class=&quot;btn btn-default&quot; <strong>role=&quot;button&quot;</strong>&gt;...&lt;/a&gt;...
&lt;/div&gt;

// Groupe de boutons justifiés&nbsp;:
&lt;div <strong>class=&quot;btn-group btn-group-justified&quot;</strong>&gt;
  &lt;div <strong>class=&quot;btn-group&quot;</strong>&gt;
    <strong>&lt;button type=&quot;button&quot; class=&quot;btn btn-default&quot;</strong>&gt;...&lt;/button&gt;
  &lt;/div&gt;...
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="btn-toolbars"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ellipsis-h fa-stack-1x fa-inverse"></span></span> Barres à outils</h4>
  <p>Utilisez pour afficher plusieurs groupes de boutons ensemble sur une seule ligne.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <ul class="btn-toolbar list-inline" role="toolbar">
            <li class="btn-group">
              <button type="button" class="btn btn-default">1</button>
              <button type="button" class="btn btn-default">2</button>
              <button type="button" class="btn btn-default">3</button>
            </li>
            <li class="btn-group">
              <button type="button" class="btn btn-default">4</button>
              <button type="button" class="btn btn-default">5</button>
            </li>
            <li class="btn-group">
              <button type="button" class="btn btn-default">6</button>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>Utilisez pour créer une barre à outils qui contient plusieurs groupes de boutons</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// Plusieurs groupes de boutons&nbsp;:
&lt;ul <strong>class=&quot;btn-toolbar list-inline&quot; role=&quot;toolbar&quot;</strong>&gt;
  &lt;li <strong>class=&quot;btn-group&quot;</strong>&gt;
   &lt;button type=&quot;button&quot; <strong>class=&quot;btn btn-default&quot;</strong>&gt;1&lt;/button&gt;
	...
  &lt;/li&gt;
  &lt;li class=&quot;btn-group&quot;&gt;
   &lt;button type=&quot;button&quot; class=&quot;btn btn-default&quot;&gt;4&lt;/button&gt;
	...
  &lt;/li&gt;
  &lt;li class=&quot;btn-group&quot;&gt;
   &lt;button type=&quot;button&quot; class=&quot;btn btn-default&quot;&gt;6&lt;/button&gt;
  &lt;/li&gt;
&lt;/ul&gt;</code></pre>
    </div>
  </div>
  <h4 id="btn-types"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-clone fa-stack-1x fa-inverse"></span></span> Genres de boutons</h4>
  <p>Utilisez  le bon texte de bouton  pour la bonne interaction avec les utilisateurs. </p>
  <div class="alert alert-info">
    <h5 class="mrgn-tp-0">Ne vous concentrez pas sur les couleurs et les styles des boutons. </h5>
    <p>Les boutons ci-dessous sont stylisés au préalable aux fins d'orientation et de démonstration.</p>
    <p>Pourvu que tous les points de conformité sur les boutons soient respectés, le bouton peut avoir différents regroupements, couleurs, tailles, <abbr title="et ainsi de suite">etc</abbr>., que ce qui est présenté.</p>
  </div>
  <table class="table table-striped table-bordered wb-tables" data-wb-tables='{"lengthMenu": [[10, -1], [10,  "All"]], "pageLength": -1 }'>
    <caption class="wb-inv">
    Genres et exemples de boutons
    </caption>
    <thead>
      <tr>
        <th scope="col">Type de bouton</th>
        <th scope="col" class="col-sm-4">Exemple</th>
        <th scope="col"><span class="nowrap">Point(s)</span> d'observation</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Bouton d'action primaire </td>
        <td><ul class="list-inline lst-spcd">
            <li>
              <button type="submit" class="btn btn-primary">Primaire </button>
            </li>
            <li>
              <button type="submit" class="btn btn-default">Secondaire</button>
            </li>
          </ul>
          <ul class="pager">
            <li class="previous"><a href="#" rel="prev">Secondaire</a></li>
            <li class="next"><a href="#" rel="next">Primaire</a></li>
          </ul>
          <hr>
          Exemple&nbsp;:
          <ul class="list-inline lst-spcd">
            <li>
              <button type="submit" class="btn btn-primary">Soumettre les changements</button>
            </li>
            <li>
              <button type="submit" class="btn btn-link">Annuler la mise à jour </button>
            </li>
          </ul>
          <ul class="list-inline lst-spcd">
            <li>
              <button type="submit" class="btn btn-success"><span class="fa fa-save"></span> Sauvegarder </button>
            </li>
            <li>
              <button type="submit" class="btn btn-default">Annuler la mise à jour</button>
            </li>
          </ul>
          <ul class="pager">
            <li class="previous"><a href="#" rel="prev">Précédent</a></li>
            <li class="next"><a href="#" rel="next">Suivant</a></li>
          </ul></td>
        <td><ul>
            <li> <strong>Mise en page type </strong>
              <ul>
                <li>Ordre par fréquence d'utilisation de gauche à droite, du plus fréquent au moins fréquent (<strong>bouton le plus à gauche =  bouton d'action primaire</strong>)</li>
                <li>Il s'agit du bouton le plus exécutable sur une page</li>
                <li>Est déclenché lorsqu'on appuie sur la touche  <kbd>Entre</kbd> dans une zone de formulaire</li>
              </ul>
            </li>
            <li><strong>Exception  </strong>
              <ul>
                <li>Utilisation de la  pagination − le bouton «&nbsp;Suivant&nbsp;» (qui se trouve <strong>à droite</strong>), est le principal bouton d'action</li>
              </ul>
            </li>
          </ul></td>
      </tr>
      <tr>
        <td>Ouvrir une session </td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-primary">Ouvrir une session </button>
            </li>
            <li>
              <button type="submit" class="btn btn-primary"><span class="fas fa-sign-in-alt"></span> Ouvrir une session </button>
            </li>
            <li>
              <button type="submit" class="btn btn-primary"><span class="="glyphicon glyphicon-off"></span> Ouvrir une session </button>
            </li>
            <li>Texte seulement&nbsp;: <a href="#"><span class="fas fa-sign-in-alt"></span> Ouvrir une session </a> ou <a href="#"> Ouvrir une session </a> </li>
          </ul></td>
        <td><ul>
            <li>Utilisez pour ouvrir une session dans une application</li>
            <li> Déterminez l'emplacement d'«&nbsp;Ouvrir une session&nbsp;» dans le cadre de l'architecture d'information du site</li>
          </ul></td>
      </tr>
      <tr>
        <td>S'inscrire</td>
        <td><button type="submit" class="btn btn-primary">S'inscrire</button></td>
        <td><ul>
            <li>Utilisez pour s'inscrire à un service ou à un programme</li>
            <li> Les nouveaux utilisateurs ne doivent pas le combiner avec «&nbsp;Ouvrir une session&nbsp;»</li>
          </ul></td>
      </tr>
      <tr>
        <td>Fermer la session </td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Fermer la session </button>
            </li>
            <li>
              <button type="submit" class="btn btn-default"><span class="fas fa-sign-out-alt"></span> Fermer la session </button>
            </li>
            <li>
              <button type="submit" class="btn btn-primary"><span class="="glyphicon glyphicon-off"></span> Fermer la session</button>
            </li>
            <li>Texte seulement : <a href="#"><span class="fas fa-sign-out-alt"></span> Fermer la session </a> or <a href="#"> Fermer une session </a> </li>
          </ul></td>
        <td><ul>
            <li>Utilisez pour fermer la session dans une  application</li>
            <li> Assurez-vous que le bouton «&nbsp;Fermer la session&nbsp;» s'affiche sur chaque page dans le coin supérieur droit pour toutes les applications qui nécessitent une ouverture de session</li>
          </ul></td>
      </tr>
      <tr>
        <td>Précédent / Suivant </td>
        <td><ul class="pager">
            <li class="previous"><a href="#" rel="prev">Précédent</a></li>
            <li class="next"><a href="#" rel="next">Suivant</a></li>
          </ul>
          <ul class="pagination">
            <li><a rel="prev" href="#">Précédent</a></li>
            <li><a href="#">1</a></li>
            <li><a href="#">2</a></li>
            <li><a href="#">3</a></li>
            <li><a rel="next" href="#">Suivant</a></li>
          </ul></td>
        <td><ul>
            <li><strong>Suivant&nbsp;: </strong>
              <ul>
                <li>Utilisez-le pour faire passer l'utilisateur à la page suivante ou à l'étape suivante du processus</li>
                <li> Il s'agit souvent du bouton d'action primaire</li>
              </ul>
            </li>
            <li><strong>Précédent&nbsp;: </strong>
              <ul>
                <li>Lisez-le pour faire passer l'utilisateur à la page suivante ou à l'étape suivante</li>
                <li>Veuillez à ce que ce soit le bouton le plus à gauche</li>
                <li>Ne l'utilisez s'il n'y a aucune page à laquelle on peut retourner (par exemple, une page d'accueil ou des pages de  confirmation)</li>
              </ul>
            </li>
          </ul>
          Pour connaître d'autres options, consultez <a href="pagination-en.html">Pagination.</a></td>
      </tr>
      <tr>
        <td>Soumettre</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Soumettre</button>
            </li>
            <li>Texte seulement : <a href="#">Soumettre</a> </li>
          </ul>
          <div class="checkbox mrgn-tp-lg">
            <label for="certified">
            <input id="certified" type="checkbox" />
            J'atteste que  <abbr title="X X X ">XXX</abbr></label>
          </div>
          <button type="submit" class="btn btn-default">Soumettre</button>
          <div class="checkbox mrgn-tp-lg">
            <label for="confirmed">
            <input id="confirmed" type="checkbox" />
            Je confirme que <abbr title="X X X ">XXX</abbr></label>
          </div>
          <button type="submit" class="btn btn-default">Soumettre</button></td>
        <td><ul>
            <li><strong>Soumettre&nbsp; </strong>
              <ul>
                <li>Utilisez-le pour envoyer des données</li>
              </ul>
            </li>
            <li><strong>Soumettre attestation </strong>
              <ul>
                <li> Utilisez-le pour obtenir une  <strong>attestation</strong> de données soumises aux fins de traitement en raison d'une incidence financière ou d'une exigence juridique</li>
                <li>Placez une case à cocher qui n'est pas étiquetée par défaut  «&nbsp;J'atteste que  <abbr title="X X X ">XXX</abbr>&nbsp;», où les  X décrivent ce qui est attesté
              <ul>
                    <li>La formulation doit être examinée par le <abbr title="Bureau de première responsabilité">BPR</abbr> opérationnel et probablement par les services juridiques</li>
                  </ul>
                </li>
                <li>Placez le bouton «&nbsp;Soumettre&nbsp;» (ou une étiquette propre à un autre contexte) sous la case à cocher
              <ul>
                    <li>Si la case à cocher d'attestation n'est pas cochée et qu'on a appuyé sur le bouton «&nbsp;Soumettre&nbsp;», affichez une erreur qui indique que la case à cocher doit être sélectionnée pour la réussite de la soumission</li>
                  </ul>
                </li>
                <li>Étiquetez la case à cocher avec le mot «&nbsp;Attester&nbsp;» si un formulaire papier connexe utilise aussi le mot «&nbsp;Attester&nbsp;»</li>
                <li>N'utilisez pas le mot «&nbsp;Attester&nbsp;» comme étiquette de bouton</li>
              </ul>
            </li>
            <li><strong>Soumettre confirmation </strong>
              <ul>
                <li> Utilisez-le pour confirmer que les données entrées sont exactes avant le traitement de la soumission</li>
                <li> Utilisez-le lorsqu'il y a peu d'incidences financières et d'exigences juridiques à remplir (au lieu de l'attestation)</li>
                <li> Placez une case à cocher qui n'est pas étiquetée par défaut « Je confirme que <abbr title="X X X ">XXX</abbr> », où les X décrivent ce qui est confirmé
                  <ul>
                    <li>La formulation doit être examinée par le <abbr title="Bureau de première responsabilité">BPR</abbr> opérationnel</li>
                  </ul>
                </li>
                <li>Placez un bouton «&nbsp;Soumettre&nbsp;» (ou une autre étiquette propre au contexte) sous la case à cocher
              <ul>
                    <li>Si la case à cocher de l'attestation n'est pas cochée et qu'on a appuyé sur «&nbsp;Soumettre&nbsp;», affichez une erreur qui indique que la case à cocher doit être sélectionnée pour la réussite de la soumission</li>
                  </ul>
                </li>
                <li> Étiquetez la case à cocher avec le mot « Confirmer » si un formulaire papier connexe utiliser aussi le mot «&nbsp;Confirmer&nbsp;»</li>
                <li> N'utilisez pas le mot «&nbsp;Confirmer&nbsp;» comme étiquette de bouton</li>
              </ul>
            </li>
          </ul></td>
      </tr>
      <tr>
        <td>Calculer</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Calculer</button>
            </li>
            <li>Texte seulement&nbsp;: <a href="#">Calculer</a> </li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le pour faire un calcul</li>
          </ul></td>
      </tr>
      <tr>
        <td>Annuler</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Annuler (x)</button>
            </li>
            <li>Texte seulement&nbsp;: <a href="#">Annuler (x)</a> </li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le prudemment pour annuler une  transaction et <strong>n'envoyez pas </strong>de renseignements</li>
            <li>Qualifiez ce qui peut être annulé si on appuie sur le bouton, par exemple, «&nbsp;Annuler la demande&nbsp;»</li>
            <li>Assurez-vous que l'utilisateur est retourné à l'endroit dans le processus s'ils ont sélectionné «&nbsp;Annuler la demande&nbsp;»</li>
            <li>Utilisez-le avec prudence
              <ul>
                <li>Il est difficile pour les utilisateurs de comprendre quelles étapes sont annulées dans un circuit de tâches qui comprennent plusieurs étapes</li>
              </ul>
            </li>
            <li>Ne faites pas de «&nbsp;Annuler la demande&nbsp;»  la touche d'action primaire</li>
          </ul></td>
      </tr>
      <tr>
        <td>Sauvegarder</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default btn-success">Sauvegarder</button>
            </li>
            <li>
              <button type="submit" class="btn btn-default btn-success"><span class="fa fa-save"></span> Sauvegarder </button>
            </li>
            <li><a href="#" class="btn btn-success"><span class="fa fa-save"></span><span class="wb-inv">Sauvegarder</span></a></li>
            <li><a href="#" class="btn btn-link"><span class="fa fa-save"></span><span class="wb-inv">Sauvegarder</span></a></li>
            <li>
              <button type="submit" class="btn btn-default">Ne pas sauvegarder </button>
            </li>
            <li>Texte seulement&nbsp;: <a href="#">Sauvegarder</a> <a href="#"><span class="fa fa-save"></span> Sauvegarder</a> ou <a href="#">Ne pas sauvegarder </a></li>
          </ul></td>
        <td><ul>
            <li><strong>Sauvegarder </strong>
              <ul>
                <li>Utilisez-le pour explicitement apporter des changements à une page ou à une séquence de pages, à la base de données ou à la  session</li>
              </ul>
            </li>
            <li class="mrgn-tp-md"><strong>Ne pas sauvegarder </strong>
              <ul>
                <li>Utilisez-le pour explicitement <strong>ne pas apporter </strong>de changements à une page ou à une séquence de  pages</li>
              </ul>
            </li>
          </ul></td>
      </tr>
      <tr>
        <td>Ajouter</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Ajouter</button>
            </li>
            <li>
              <button type="submit" class="btn btn-default"><span class="fa fa-plus"></span> Ajouter </button>
            </li>
            <li>
              <button type="submit" class="btn btn-default"><span class="fa fa-plus"></span> Ajouter (enfant)</button>
            </li>
            <li><a href="#" class="btn btn-default"><span class="fa fa-plus"></span><span class="wb-inv">Ajouter</span></a></li>
            <li><a href="#" class="btn btn-link"><span class="fa fa-plus"></span><span class="wb-inv">Ajouter</span></a></li>
            <li>Texte seulement&nbsp;: <a href="#">Ajouter</a>, <a href="#"><span class="fa fa-plus"></span> Ajouter</a> ou <a href="#"><span class="fa fa-plus"></span> Ajouter (enfant)</a></li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le pour ajouter ou insérer un  item, par exemple, ajouter une adresse
              <ul>
                <li> S'il y a lieu, précisez ce qui est ajouté dans le cadre du nom du bouton</li>
              </ul>
            </li>
            <li>Utilisez-le dans un processus de liste pour ajouter un autre item à une liste</li>
          </ul></td>
      </tr>
      <tr>
        <td>Modifier</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default"><span class="fa fa-edit"></span> Modifier </button>
            </li>
            <li>
              <button type="submit" class="btn btn-default"><span class="fa fa-edit"></span> Modifier (x)</button>
            </li>
            <li><a href="#" class="btn btn-default"><span class="fa fa-edit"></span><span class="wb-inv">Modifier</span></a></li>
            <li><a href="#" class="btn btn-link"><span class="fa fa-edit"></span><span class="wb-inv">Modifier</span></a></li>
            <li>Texte seulement : <a href="#">Modifier</a> ou <a href="#"><span class="fa fa-edit"></span> Modifier </a></li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le pour modifier  un item, par exemple, modifier une adresse
              <ul>
                <li> S'il y a lieu, précisez ce qui est modifié dans le cadre du nom du bouton</li>
              </ul>
            </li>
            <li> Utilisez-le dans un processus de liste pour modifier l'item sélectionné dans une liste</li>
          </ul></td>
      </tr>
      <tr>
        <td>Supprimer</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-warning">Supprimer</button>
            </li>
            <li>
              <button type="submit" class="btn btn-warning">Supprimer (x)</button>
            </li>
            <li>
              <button type="submit" class="btn btn-warning"><span class="fas fa-trash-alt"></span> Supprimer </button>
            </li>
            <li>
              <button type="submit" class="btn btn-warning"><span class="fas fa-trash-alt"></span> Supprimer (x)</button>
            </li>
            <li><a href="#" class="btn btn-warning"><span class="fas fa-trash-alt"></span><span class="wb-inv">Supprimer</span></a></li>
            <li><a href="#" class="btn btn-link"><span class="fas fa-trash-alt"></span><span class="wb-inv">Supprimer</span></a></li>
            <li>Texte seulement&nbsp;: <a href="#">Supprimer</a>, <a href="#">Supprimer (x)</a>, <a href="#"><span class="fas fa-trash-alt"></span> Supprimer</a> ou <a href="#"><span class="fas fa-trash-alt"></span> Supprimer (x)</a></li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le pour supprimer un item, par exemple, supprimer une adresse
              <ul>
                <li>S'il y a lieu, précisez ce qui est supprimé dans le cadre du nom du bouton</li>
              </ul>
            </li>
            <li>Utilisez-le dans un processus de liste pour supprimer l'item sélectionné dans une liste</li>
          </ul></td>
      </tr>
      <tr>
        <td>Afficher</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Afficher</button>
            </li>
            <li>
              <button type="submit" class="btn btn-default">Afficher en <abbr title="format de document portable">PDF</abbr></button>
            </li>
            <li>Texte seulement&nbsp;: <a href="#">Afficher</a> ou <a href="#">Afficher en <abbr title="format de document portable">PDF</abbr></a></li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le pour voir un item comme l'affichage du statut d'une demande
              <ul>
                <li>S'il y a lieu, précisez ce qui est affiché dans le cadre du nom du bouton</li>
              </ul>
            </li>
          </ul></td>
      </tr>
      <tr>
        <td>Extraire </td>
        <td><button type="submit" class="btn btn-default">Extraire</button></td>
        <td><ul>
            <li>Utilisez-le pour extraire un item, par exemple, extraire une adresse
              <ul>
                <li>S'il y a lieu, précisez ce qui est extrait dans le cadre du nom du bouton</li>
              </ul>
            </li>
          </ul></td>
      </tr>
      <tr>
        <td>Rechercher</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Rechercher</button>
            </li>
            <li>
              <button type="submit" class="btn btn-default"><span class="fa fa-search"></span> Rechercher </button>
            </li>
            <li><a href="#" class="btn btn-default"><span class="fa fa-search"></span><span class="wb-inv">Rechercher</span></a></li>
            <li><a href="#" class="btn btn-link"><span class="fa fa-search"></span><span class="wb-inv">Rechercher</span></a></li>
            <li>Texte seulement : <a href="#">Rechercher</a> ou <a href="#"><span class="fa fa-search"></span> Rechercher </a></li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le pour faire une recherche</li>
          </ul></td>
      </tr>
      <tr>
        <td>Réinitialiser</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Réinitialiser</button>
            </li>
            <li>Aucun bouton : <a href="#">Réinitialiser</a></li>
          </ul></td>
        <td><ul>
            <li>Utilisez-le pour réinitialiser toutes les zones sur une  page (sur le côté du client) pour les valeurs initiales au moment où la page a été chargée au départ</li>
            <li>Demandez exactement aux utilisateurs ce qui est réinitialisé si la réinitialisation s'étend sur plus d'une page (par exemple, «&nbsp;Réinitialiser la page aux valeurs par défaut&nbsp;»)</li>
            <li> Évitez de placer le bouton «&nbsp;Réinitialiser&nbsp;»  pour les raisons suivantes&nbsp;:
              <ul>
                <li>les utilisateurs peuvent cliquer sur le bouton par erreur;</li>
                <li>les utilisateurs n'ont pas besoin d'options inutiles pour encombrer l'interface et qui requièrent plus de temps de réflexion</li>
              </ul>
            </li>
          </ul></td>
      </tr>
      <tr>
        <td>Recommencer</td>
        <td><button type="submit" class="btn btn-default">Recommencer</button></td>
        <td><ul>
            <li>Utilisez-le lorsque les utilisateurs doivent recommencer à partir de l'étape&nbsp;1 selon une séquence d'étapes</li>
          </ul></td>
      </tr>
      <tr>
        <td>Imprimer</td>
        <td><ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Imprimer</button>
            </li>
            <li>
              <button type="submit" class="btn btn-default"><span class="fa fa-print"></span> Imprimer </button>
            </li>
            <li><a href="#" class="btn btn-default"><span class="fa fa-print"></span><span class="wb-inv">Imprimer</span></a></li>
            <li><a href="#" class="btn btn-link"><span class="fa fa-print"></span><span class="wb-inv">Imprimer</span></a></li>
            <li>Aucun bouton&nbsp;: <a href="#">Imprimer</a> ou <a href="#"><span class="fa fa-print"></span> Imprimer </a></li>
          </ul></td>
        <td><ul>
            <li> Ne l'utilisez que dans les  situations où il est nécessaire de demander à l'utilisateur d'imprimer quelque chose d'important (telle qu'une page de confirmation avec un numéro de  confirmation ou de référence)
              <ul>
                <li>Un utilisateur peut utiliser la fonction d'impression dans son navigateur afin d'imprimer la page courante</li>
              </ul>
            </li>
            <li>Utilisez «&nbsp;Afficher en <abbr title="format de document portable">PDF</abbr>&nbsp;» si l'action souhaitée est de charger le document en <abbr title="format de document portable">PDF</abbr> pour le consulter (puis de l'imprimer au besoin)</li>
          </ul></td>
      </tr>
      <tr>
        <td>Effacer</td>
        <td><ul class="list-unstyled lst-spcd">
            <li><span class="pull-right text-danger"><span class="fa-stack fa-lg"> <span class="fa fa-circle fa-stack-2x text-danger"></span> <span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Ne pas utiliser </span>
              <button type="submit" class="btn btn-default">Effacer</button>
            </li>
          </ul></td>
        <td><ul>
            <li> N'utilisez pas le bouton «&nbsp;Effacer&nbsp;»</li>
            <li>Reportez-vous à la section sur le bouton «&nbsp;Réinitialiser&nbsp;»</li>
          </ul></td>
      </tr>
      <tr>
        <td>Sortir <br>
          Quitter</td>
        <td><span class="pull-right text-danger"><span class="fa-stack fa-lg"> <span class="fa fa-circle fa-stack-2x text-danger"></span> <span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Ne pas utiliser </span>
          <ul class="list-unstyled lst-spcd">
            <li>
              <button type="submit" class="btn btn-default">Sortir</button>
            </li>
            <li>
              <button type="submit" class="btn btn-default">Quitter</button>
            </li>
          </ul></td>
        <td><ul>
            <li>N'utilisez pas les boutons «&nbsp;Sortir&nbsp;» ou «&nbsp;Quitter&nbsp;», car ils sont redondants
              <ul>
                <li>Les utilisateurs ferment souvent la fenêtre de leur navigateur pour sortir d'une application</li>
              </ul>
            </li>
            <li>Utilisez  le bouton «&nbsp;Fermer la session&nbsp;» pour les applications qui nécessitent une ouverture de session</li>
            <li>Envisagez d'utiliser le bouton «&nbsp;Annuler&nbsp; <abbr title="X X X ">XXX</abbr>&nbsp;», car il peut être plus approprié selon l'exigence de l'application</li>
          </ul></td>
      </tr>
      <tr>
        <td>Je suis d'accord </td>
        <td><span class="pull-right text-danger"><span class="fa-stack fa-lg"> <span class="fa fa-circle fa-stack-2x text-danger"></span> <span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Ne pas utiliser </span>
          <ul class="list-unstyled lst-spcd">
            <li>
              <div class="checkbox">
                <label for="agreed">
                <input id="agreed" type="checkbox" />
                Je suis d'accord </label>
              </div>
            </li>
            <li>
              <button type="submit" class="btn btn-default">Je suis d'accord </button>
            </li>
          </ul></td>
        <td><ul>
            <li> N'utilisez pas la case à cocher ou le bouton «&nbsp;Je suis d'accord&nbsp;» afin de confirmer que la saisie de données est exacte
              <ul>
                <li>L'expression «&nbsp;Je suis d'accord&nbsp;» est principalement associée avec l'«&nbsp;avis de non-responsabilité&nbsp;» qui est présenté à l'utilisateur avant de lancer l'application</li>
              </ul>
            </li>
            <li>Reportez-vous à la section sur les fonctions «&nbsp;Confirmer&nbsp;» et «&nbsp;Attester&nbsp;»</li>
          </ul></td>
      </tr>
    </tbody>
  </table>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Caractéristiques additionnelles </h4>
  <p>Des fonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="pagination-en.html">Pagination</a></li>
    <li><a class="btn btn-default" href="icons-en.html">Icônes</a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
