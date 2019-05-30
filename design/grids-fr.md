---
published: true
layout: default-theme-wet-boew-fr
title: Grilles
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
            <li><a href="#design">Conception et codage </a>
              <ul>
                <li><a href="#basic">Utilisation de base </a>
                  <ul>
                    <li><a href="#responsive">Options de grilles souples</a></li>
                    <li><a href="#basic">Rangée d'une grille de base</a></li>
                    <li><a href="#fluid">Conteneur fluide </a></li>
                  </ul>
                </li>
                <li><a href="#enhanced">Utilisation améliorée</a>
                  <ul>
                    <li><a href="#mixed">Appareils mobiles et ordinateurs de bureau </a></li>
                    <li><a href="#mixed-complete">Appareils mobiles, tablettes et ordinateurs de bureau</a></li>
                    <li><a href="#resets">Réinitialisation de colonnes souples</a></li>
                    <li><a href="#offsetting">Décalage de colonnes</a></li>
                    <li><a href="#nesting">Imbrication de colonnes</a></li>
                    <li><a href="#ordering">Ordonnancement de colonnes</a></li>
                    <li><a href="#addon">Caractéristiques complémentaires </a> </li>
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
          <p>Veuillez  <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème </a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage </h2>
  <p>Utiliser un système de grille (une série de rangées et de colonnes qui hébergent du contenu) afin de créer de la mise en page. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base </h3>
  <h4 id="responsive"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Options de grilles souples </h4>
  <p>Utilisez un système de grilles afin de créer un système de grille souple, fluide et mobile d'abord. Il met à l'échelle jusqu'à 12 colonnes environ, au fur et à mesure que la taille de l'appareil ou de la fenêtre d'affichage augmente.</p>
  <ul>
    <li>Placez les rangées dans  <code>.container</code> (largeur fixe) ou <code>.container-fluid</code> (pleine largeur) pour un alignement et un remplissage appropriés</li>
    <li>Utilisez des rangées pour créer des groupes  de colonnes horizontales</li>
    <li>Placez le contenu dans les colonnes
              <ul>
        <li>Seules les colonnes peuvent être des enfants immédiats de rangées</li>
        <li>Les colonnes créent des gouttières (un espacement entre les colonnes) par <code>padding:</code> de <abbr title="feuille de style en cascade">CSS</abbr>. Ce remplissage est souvent décalé dans les rangées pour la première et dernière colonnes à l'aide d'un marge négative sur <code>.row</code></li>
      </ul>
    </li>
    <li>Précisez le nombre   à étendre (parmi 12 colonnes disponibles)  afin de créer des colonnes de grille. Par exemple, pour trois colonnes égales utilisez trois  <code>.col-xs-4</code>
              <ul>
        <li>Les catégories de grilles s'appliquent aux appareils ayant des largeurs supérieures ou égales aux tailles de point d'interruption et remplacent les catégories de grille  ciblant des appareils plus petits</li>
        <li>L'application de  toute catégorie <code>.col-md-</code> à un élément a une incidence sur la stylisation sur les appareils moyens ainsi que sur les grands  si une catégorie <code>.col-lg-</code> ne s'y trouve pas</li>
      </ul>
    </li>
    <li>Créez des mises en page entièrement fluides (le site Web s'étend sur toute la largeur de la fenêtre d'affichage)
              <ul>
        <li>Pour ce faire, enveloppez le contenu de la grille dans un élément du conteneur avec <code>padding: 0 15px;</code> afin de décaler  <code>margin: 0 -15px;</code> sur <code>.row</code> </li>
      </ul>
    </li>
  </ul>
  <div class="table-responsive">
    <table class="table table-bordered table-striped">
      <caption>
      Options souples
      </caption>
      <thead>
        <tr>
          <td></td>
          <th scope="col"> Téléphones – appareils <small> très petits (&lt;768 px)</small></th>
          <th scope="col"><small>Tablettes – appareils petits (=768 px)</small></th>
          <th scope="col">Ordinateurs de bureau – appareils de taille moyenne<small> (=992 px)</small></th>
          <th scope="col">Ordinateurs de bureau – grands appareil<small>s (=1200 px)</small></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">Comportement de grille</th>
          <td>Horizontal en tout temps </td>
          <td colspan="3">Réduit pour commencer et horizontal au-dessus des points d'interruption </td>
        </tr>
        <tr>
          <th scope="row">Largeur des conteneurs </th>
          <td>Aucune (automatique)</td>
          <td>750px</td>
          <td>970px</td>
          <td>1170px</td>
        </tr>
        <tr>
          <th scope="row">Préfixe de catégorie  </th>
          <td><code>.col-xs-</code></td>
          <td><code>.col-sm-</code></td>
          <td><code>.col-md-</code></td>
          <td><code>.col-lg-</code></td>
        </tr>
        <tr>
          <th scope="row">Nombre de colonnes</th>
          <td colspan="4">12</td>
        </tr>
        <tr>
          <th scope="row">Largeur de la colonne</th>
          <td class="text-muted">Automatique</td>
          <td>60px</td>
          <td>78px</td>
          <td>95px</td>
        </tr>
        <tr>
          <th scope="row">Largeur de la gouttière</th>
          <td colspan="4">30px (15px sur chaque côté d'une colonne)</td>
        </tr>
        <tr>
          <th scope="row">Emboîtable</th>
          <td colspan="4">Oui</td>
        </tr>
        <tr>
          <th scope="row">Décalages</th>
          <td colspan="4">Oui</td>
        </tr>
        <tr>
          <th scope="row">Ordonnancement des colonnes</th>
          <td colspan="4">Oui</td>
        </tr>
      </tbody>
    </table>
  </div>
  <h4 id="row"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-desktop fa-stack-1x fa-inverse"></span></span> Rangée d'une grille de base </h4>
  <p>Utilisez un seul ensemble de catégories de grille <code>.col-md-*</code> afin de créer un système de grille de base qui commence  empilé sur les appareils mobiles et les  tablettes (de taille très petite à petite). Il commence ensuite horizontal sur des appareils d'ordinateur de bureau (moyen). Placez des colonnes de grille dans n'importe quelle rangée <code>.row</code>.</p>
  <div class="row">
    <div class="col-md-7">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="text-center">
            <div class="row">
              <div class="col-md-2">
                <div class="well well-sm brdr-rds-0"><code>.col-md-2</code></div>
              </div>
              <div class="col-md-2">
                <div class="well well-sm brdr-rds-0"><code>.col-md-2</code></div>
              </div>
              <div class="col-md-2">
                <div class="well well-sm brdr-rds-0"><code>.col-md-2</code></div>
              </div>
              <div class="col-md-2">
                <div class="well well-sm brdr-rds-0"><code>.col-md-2</code></div>
              </div>
              <div class="col-md-2">
                <div class="well well-sm brdr-rds-0"><code>.col-md-2</code></div>
              </div>
              <div class="col-md-2">
                <div class="well well-sm brdr-rds-0"><code>.col-md-2</code></div>
              </div>
            </div>
            <div class="row">
              <div class="col-md-8">
                <div class="well well-sm brdr-rds-0"><code>.col-md-8</code></div>
              </div>
              <div class="col-md-4">
                <div class="well well-sm brdr-rds-0"><code>.col-md-4</code></div>
              </div>
            </div>
            <div class="row">
              <div class="col-md-4">
                <div class="well well-sm brdr-rds-0"><code>.col-md-4</code></div>
              </div>
              <div class="col-md-4">
                <div class="well well-sm brdr-rds-0"><code>.col-md-4</code></div>
              </div>
              <div class="col-md-4">
                <div class="well well-sm brdr-rds-0"><code>.col-md-4</code></div>
              </div>
            </div>
            <div class="row">
              <div class="col-md-6">
                <div class="well well-sm brdr-rds-0"><code>.col-md-6</code></div>
              </div>
              <div class="col-md-6">
                <div class="well well-sm brdr-rds-0"><code>.col-md-6</code></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <details>
        <summary>Code</summary>
        <pre><code>&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-md-2&quot;</strong>&gt;
   ...
  &lt;/div&gt;
  &lt;div class=&quot;col-md-2&quot;&gt;
   ...
  &lt;/div&gt;
  &lt;div class=&quot;col-md-2&quot;&gt;
   ...
  &lt;/div&gt;
  &lt;div class=&quot;col-md-2&quot;&gt;
   ...
  &lt;/div&gt;
  &lt;div class=&quot;col-md-2&quot;&gt;
   ...
  &lt;/div&gt;
  &lt;div class=&quot;col-md-2&quot;&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;

&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-md-8&quot;</strong>&gt;
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-md-4&quot;</strong>&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;

&lt;div class=&quot;row&quot;&gt;
  &lt;div<strong> class=&quot;col-md-4&quot;</strong>&gt;
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-md-4</strong>&quot;&gt;
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-md-4&quot;</strong>&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;

&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-md-6&quot;</strong>&gt;
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-md-6&quot;</strong>&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="fluid"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-h fa-stack-1x fa-inverse"></span></span> Conteneur fluide</h4>
  <p>Utilisez pour  transformer n'importe quelle mise en page de grille à largeur fixe en  mise en page de pleine largeur. Changez le <code>.container</code> le plus à l'extérieur pour  <code>.container-fluid</code>.</p>
  <h5 class="mrgn-tp-0">Code</h5>
  <pre><code>&lt;div <strong>class=&quot;container-fluid&quot;</strong>&gt;
	&lt;div class=&quot;row&quot;&gt;
		...
	&lt;/div&gt;
&lt;/div&gt;</code></pre>
  <h3 id="enhanced">Utilisation améliorée </h3>
  <h4 id="mixed"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-mobile-alt fa-stack-1x fa-inverse"></span></span> Appareils mobiles et ordinateurs de bureau</h4>
  <p>Utilisez-le pour empêcher les colonnes de simplement s'empiler dans des appareils plus petits. Utilisez les catégories de grille d'appareils très petits et moyens. Ajoutez <code>.col-xs-*</code> <code>.col-md-*</code> aux colonnes. Reportez-vous à l'exemple ci-dessous pour avoir une meilleure idée de son fonctionnement.</p>
  <div class="row">
    <div class="col-md-7">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="row">
            <div class="col-xs-12 col-md-8">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-12 .col-md-8</code></div>
            </div>
            <div class="col-xs-6 col-md-4">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-md-4</code></div>
            </div>
          </div>
          <div class="row">
            <div class="col-xs-6 col-md-4">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-md-4</code></div>
            </div>
            <div class="col-xs-6 col-md-4">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-md-4</code></div>
            </div>
            <div class="col-xs-6 col-md-4">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-md-4</code></div>
            </div>
          </div>
          <div class="row">
            <div class="col-xs-6">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6</code></div>
            </div>
            <div class="col-xs-6">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6</code></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <details>
        <summary>Code</summary>
        <pre><code>&lt;!-- Empiler les colonnes sur un appareil mobile en faisant une pleine largeur et l'autre, une demi-largeur --&gt;
&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-xs-12 col-md-8&quot;</strong>&gt;...&lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-md-4&quot;</strong>&gt;...&lt;/div&gt;
&lt;/div&gt;

&lt;!-- Les colonnes commencent à 50&nbsp;% de largeur sur les appareils mobiles et montent jusqu'à une largeur de 33,3&nbsp;% sur les appareils de bureau --&gt;
&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-md-4&quot;</strong>&gt;...&lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-md-4&quot;</strong>&gt;...&lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-md-4&quot;</strong>&gt;...&lt;/div&gt;
&lt;/div&gt;

&lt;!-- Les colonnes ont toujours une largeur de 50&nbsp;% sur les appareils mobiles et les ordinateurs de bureau --&gt;
&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-xs-6&quot;</strong>&gt;...&lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6&quot;</strong>&gt;...&lt;/div&gt;
&lt;/div&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="mixed-complete"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-tablet-alt fa-stack-1x fa-inverse"></span></span> Appareils mobiles, tablettes et ordinateurs de bureau</h4>
  <p>Utilisez pour créer des mises en page encore plus dynamiques et puissantes avec des catégories <code>.col-sm-*</code> de tablette.</p>
  <div class="row">
    <div class="col-md-7">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="row">
            <div class="col-xs-12 col-sm-6 col-md-8">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-12 .col-sm-6 .col-md-8</code></div>
            </div>
            <div class="col-xs-6 col-md-4">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-md-4</code></div>
            </div>
          </div>
          <div class="row">
            <div class="col-xs-6 col-sm-4">
              <div class="well well-sm brdr-rds-0"><code>col-xs-6 .col-sm-4</code></div>
            </div>
            <div class="col-xs-6 col-sm-4">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-sm-4</code></div>
            </div>
            <!-- Optional: clear the XS cols if their content doesn't match in height -->
            <div class="clearfix visible-xs"></div>
            <div class="col-xs-6 col-sm-4">
              <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-sm-4</code></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <details>
        <summary>Code</summary>
        <pre><code>&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-xs-12 col-sm-6 col-md-8&quot;</strong>&gt;
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-md-4&quot;</strong>&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;
&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-sm-4&quot;</strong>&gt;
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-sm-4&quot;</strong>&gt;
   ...
  &lt;/div&gt;

  &lt;!-- facultatif : effacez les colonnes XS si leur contenu n'est pas de la même hauteur --&gt;
  &lt;div <strong>class=&quot;clearfix visible-xs&quot;</strong>&gt;&lt;/div&gt;

  &lt;div class=&quot;col-xs-6 col-sm-4&quot;&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;
</code></pre>
      </details>
    </div>
  </div>
  <h4 id="resets"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-ban fa-stack-1x fa-inverse"></span></span> Réinitialisation de colonnes souples </h4>
  <p>Utilisez pour forcer des points d'interruption dans le contenu. Avec les quatre niveaux de grille disponibles, des problèmes peuvent survenir.  À certains points d'interruption, les colonnes ne s'effacent pas toujours convenablement, par exemple, si une colonne est plus haute que l'autre. Pour corriger ce problème, utilisez une combinaison de  <code>.clearfix</code> et de <a href="visible-fr.html"> catégories invisibles et visibles</a>.</p>
  <div class="row">
    <div class="col-md-7">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="text-center">
            <div class="row">
              <div class="col-xs-6 col-sm-3">
                <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-sm-3</code><br />
                  Redimensionnez la fenêtre d'affichage ou vérifiez-la sur un téléphone cellulaire par exemple. </div>
              </div>
              <div class="col-xs-6 col-sm-3">
                <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-sm-3</code></div>
              </div>
              <!-- Add the extra clearfix for only the required viewport -->
              <div class="clearfix visible-xs"></div>
              <div class="col-xs-6 col-sm-3">
                <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-sm-3</code></div>
              </div>
              <div class="col-xs-6 col-sm-3">
                <div class="well well-sm brdr-rds-0"><code>.col-xs-6 .col-sm-3</code></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <details>
        <summary>Code</summary>
        <pre><code>&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-sm-3&quot;&gt;</strong>
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-sm-3&quot;</strong>&gt;
   ...
  &lt;/div&gt;

  &lt;!-- Ajoutez une autre fonction d'effacement total pour seulement la fenêtre d'affichage requis --&gt;
  &lt;div <strong>class=&quot;clearfix visible-xs&quot;</strong>&gt;&lt;/div&gt;

  &lt;div <strong>class=&quot;col-xs-6 col-sm-3&quot;</strong>&gt;
   ...
  &lt;/div&gt;
  &lt;div <strong>class=&quot;col-xs-6 col-sm-3&quot;</strong>&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;
</code></pre>
      </details>
    </div>
  </div>
  <h5>Réinitialisation des décalages, pousser (<span lang="en">pushes</span>) et tirer (<span lang="en">pulls</span>)</h5>
  <p>Utilisez la réinitialisation des <strong>décalages, de pousser et de tirer</strong> en plus de l'effacement de colonne aux points d'interruption souples. La réinitialisation est disponible pour <strong>les niveaux de grille moyenne et grande seulement</strong> puisqu'ils commencent au niveau de petite grille (deuxième niveau). Reportez-vous à l'exemple de grille.</p>
  <div class="mrgn-tp-lg">
    <pre><code>&lt;div class=&quot;row&quot;&gt;
	&lt;div class=&quot;col-sm-5 col-md-6&quot;&gt;.col-sm-5 .col-md-6&lt;/div&gt;
	&lt;div class=&quot;col-sm-5 <strong>col-sm-offset-2</strong> col-md-6 <strong>col-md-offset-0&quot;</strong>&gt;.col-sm-5 .col-sm-offset-2 .col-md-6 .col-md-offset-0&lt;/div&gt;
&lt;/div&gt;
&lt;div class=&quot;row&quot;&gt;
	&lt;div class=&quot;col-sm-6 col-md-5 col-lg-6&quot;&gt;.col-sm-6 .col-md-5 .col-lg-6&lt;/div&gt;
	&lt;div class=&quot;col-sm-6 col-md-5 <strong>col-md-offset-2</strong> col-lg-6 <strong>col-lg-offset-0</strong>&quot;&gt;.col-sm-6 .col-md-5 .col-md-offset-2 .col-lg-6 .col-lg-offset-0&lt;/div&gt;
&lt;/div&gt;</code></pre>
  </div>
  <h4 id="offsetting"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8614;</span></span> Décaler des colonnes</h4>
  <p>Utilisez pour déplacer les colonnes à droite avec la catégorie <code>.col-md-offset-*</code>. Ces catégories augmentent la marge de gauche d'une colonne par les colonnes <code>*</code>. Par exemple, <code>.col-md-offset-4</code> déplace <code>.col-md-4</code> sur quatre colonnes.</p>
  <div class="row">
    <div class="col-md-7">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="text-center">
            <div class="row">
              <div class="col-md-4">
                <div class="well well-sm brdr-rds-0"><code>.col-md-4</code></div>
              </div>
              <div class="col-md-4 col-md-offset-4">
                <div class="well well-sm brdr-rds-0"><code>.col-md-4 .col-md-offset-4</code></div>
              </div>
            </div>
            <div class="row">
              <div class="col-md-3 col-md-offset-3">
                <div class="well well-sm brdr-rds-0"><code>.col-md-3 .col-md-offset-3</code></div>
              </div>
              <div class="col-md-3 col-md-offset-3">
                <div class="well well-sm brdr-rds-0"><code>.col-md-3 .col-md-offset-3</code></div>
              </div>
            </div>
            <div class="row">
              <div class="col-md-6 col-md-offset-3">
                <div class="well well-sm brdr-rds-0"><code>.col-md-6 .col-md-offset-3</code></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <details>
        <summary>Code</summary>
        <pre><code>&lt;div class=&quot;row&quot;&gt;
  &lt;div class=&quot;col-md-4&quot;&gt;
   ...
  &lt;/div&gt;
  &lt;div class=&quot;col-md-4 <strong>col-md-offset-4</strong>&quot;&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;
&lt;div class=&quot;row&quot;&gt;
  &lt;div class=&quot;col-md-3 <strong>col-md-offset-3</strong>&quot;&gt;
   ...
  &lt;/div&gt;
  &lt;div class=&quot;col-md-3 <strong>col-md-offset-3</strong>&quot;&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;
&lt;div class=&quot;row&quot;&gt;
  &lt;div class=&quot;col-md-6 <strong>col-md-offset-3</strong>&quot;&gt;
   ...
  &lt;/div&gt;
&lt;/div&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="nesting"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-table fa-stack-1x fa-inverse"></span></span> Imbrication de colonnes</h4>
  <p>Utilisez pour imbriquer le contenu avec la grille par défaut. Ajoutez une nouvelle <code>.row</code> et un ensemble de colonnes  <code>.col-md-*</code>  dans la colonne <code>.col-md-*</code> existante. Les colonnes imbriquées devraient inclure un ensemble de colonnes qui s'accumulent jusqu'à 12.</p>
  <div class="row">
    <div class="col-md-7">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="row">
            <div class="col-md-9">
              <div class="brdr-tp brdr-lft brdr-bttm brdr-rght">
                <p class="mrgn-tp-md mrgn-lft-md mrgn-bttm-md">Niveau 1&nbsp;: <code>.col-md-9</code></p>
                <div class="row">
                  <div class="col-md-6">
                    <div class="well well-sm brdr-rds-0">Niveau 2&nbsp;: <code>.col-md-6</code></div>
                  </div>
                  <div class="col-md-6">
                    <div class="well well-sm brdr-rds-0">Niveau 2&nbsp;: <code>.col-md-6</code></div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <details>
        <summary>Code</summary>
        <pre><code>&lt;div class=&quot;row&quot;&gt;
  &lt;div <strong>class=&quot;col-md-9&quot;</strong>&gt;
   &lt;div class=&quot;row&quot;&gt;
    &lt;div <strong>class=&quot;col-md-6&quot;</strong>&gt;
     ...
    &lt;/div&gt;
    &lt;div <strong>class=&quot;col-md-6&quot;</strong>&gt;
     ...
    &lt;/div&gt;
   &lt;/div&gt;
  &lt;/div&gt;
&lt;/div&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="ordering"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8633; </span></span> Ordonnancement de colonnes </h4>
  <p>Utilisez-le pour facilement changer l'ordre des colonnes de grille intégrées par les catégories de modificateur <code>.col-md-push-*</code> et <code>.col-md-pull-*</code>.</p>
  <div class="row">
    <div class="col-md-7">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="row">
            <div class="col-md-9 col-md-push-3">
              <div class="well well-sm brdr-rds-0"><code>.col-md-9 .col-md-push-3</code></div>
            </div>
            <div class="col-md-3 col-md-pull-9">
              <div class="well well-sm brdr-rds-0"><code>.col-md-3 .col-md-pull-9</code></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <details>
        <summary>Code</summary>
        <pre><code>&lt;div class=&quot;row&quot;&gt;
	&lt;div class=&quot;col-md-9 <strong>col-md-push-3</strong>&quot;&gt;.col-md-9 .col-md-push-3&lt;/div&gt;
	&lt;div class=&quot;col-md-3 <strong>col-md-pull-9</strong>&quot;&gt;.col-md-3 .col-md-pull-9&lt;/div&gt;
&lt;/div&gt;</code></pre>
      </details>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires</h4>
  <p>Des fonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="reflow-fr.html">Redistribuer le contenu autour des grilles</a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" rel="external">Bootstrap<span class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
