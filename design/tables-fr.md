---
published: true
layout: default-theme-wet-boew-fr
title: Tableaux
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
                <li><a href="#enhanced">Utilisation améliorée</a>
                  <ul>
                    <li><a href="#width">Modifier la largeur des colonnes et des tableaux</a></li>
                    <li><a href="#striped">Rangées rayées (Zébrures)</a></li>
                    <li><a href="#hover">Rangées à pointage</a></li>
                    <li><a href="#bordered">Rangées à bordure</a></li>
                    <li><a href="#condensed">Rangées condensées</a></li>
                    <li><a href="#responsive">Tableaux réactifs</a></li>
                    <!--  <li><a href="#gridify">Gridify table</a></li> -->
                    <li><a href="#colours">Rangées et cellules colorées </a></li>
                    <li><a href="#addon">Fonctions complémentaires</a></li>
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
  <p>Les utiliser pour organiser les données en rangées et en colonnes afin de créer des cellules de données. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base</h3>
  <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Défaut</h4>
  <p>Les utiliser pour appliquer un style de base (seulement les séparateurs horizontaux et le remplissage léger). Ajoutez le <abbr title="feuille de style en cascade">CSS</abbr> de base  <code>.table</code> à n'importe quelle balise de tableau <code>&lt;table&gt;</code>. Vu la grande popularité des tableaux pour d'autres plugiciels comme les calendriers et les sélecteurs de date, cette page énumère des styles de tableau personnalisés isolés.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <h6  class="h5 mrgn-tp-xl">En-tête au-dessus du tableau</h6>
          <table class="table">
            <caption class="wb-inv">
            Exemple de tableau avec en-tête
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
            </tbody>
          </table>
          <h6  class="h5 mrgn-tp-xl">Cellules vides dans un tableau </h6>
          <table class="table">
            <caption class="wb-inv">
            Exemple de tableau avec des cellules de données invisibles
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>-</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>-</td>
              </tr>
            </tbody>
          </table>
          <table class="table">
            <caption>
            Légende du tableau
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez des tableaux pour afficher des données tabulaires comme des renseignements financiers, statistiques, comparatifs ou numériques</li>
        <li>Utilisez <code>.table</code> pour appliquer un style de tableau de base</li>
        <li>Utilisez du texte d'en-tête uniforme dans les tableaux liés
          <ul>
            <li>Par exemple, utilisez l'en-tête « Nom » pour la liste de toutes les personnes-ressources, et non divers titres comme « Personnes-ressources », « Nom » ou « Utilisateur »</li>
          </ul>
        </li>
        <li>Insérez  <strong>un trait d'union  (-) </strong> dans les cellules de données vides
          <ul>
            <li>Le trait d'union (-) permet au lecteur d'écran de lire correctement le contenu comme étant « vide », et il s'affiche correctement lorsqu'il est grossi</li>
          </ul>
        </li>
        <li>Incluez l'élément approprié <code>scope=&quot;col&quot;</code> ou <code>scope=&quot;row"</code> dans la balise <code>&lt;th&gt;</code></li>
        <li>Insérez une balise de titre descriptive <code>&lt;h*&gt;</code><strong>directement au-dessus</strong> d'un tableau lorsque celui-ci ne comporte pas de balise  <code>&lt;caption&gt;</code></li>
        <li>Incluez une  tableau légende visible  lorsque le titre de <code>&lt;h*&gt;</code> ne se trouve pas directement au-dessus du tableau, ou  <strong>si plusieurs tableaux apparaissent en-dessous  </strong>d'une balise <code>&lt;h*&gt;</code>
          <ul>
            <li>Utilisez une balise <code>&lt;caption&gt;</code> sur toutes les tableaux afin qu'ils valident et, en plus d'être accessible et descriptif (surtout dans des pages statistiques ou financières qui comportent plusieurs tableaux)</li>
            <li>Utilisez <code>.wb-inv</code> (au besoin) pour rendre invisible la légende du tableau, tout en assurant cependant l'accessibilité</li>
          </ul>
        </li>
        <li>Comprenez et mettez en œuvre les <a href="#supporting"> principes à l'appui</a> connexes</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
        <li>N'utilisez pas les tableaux à des fins de mise en page</li>
        <li>N'utilisez pas <code>title=&quot;&quot;</code> à l'intérieur de la balise <code>&lt;table&gt;</code></li>
        <li>À l'intérieur d'un tableau, n'inscrivez pas <abbr title="Sans objet">S.O.</abbr> ou   <code>&amp;nbsp;</code> ne laissez pas non plus de cellules vides
          <ul>
            <li>Ceci empêchera les problèmes liés aux lecteurs d'écran</li>
          </ul>
        </li>
        <li>Évitez les cellules fusionnées, puisqu'elles sont complexes à coder et qu'elles présentent des problèmes d'accessibilité</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>// En-tête au-dessus d'un tableau :
<strong>&lt;h*&gt;...&lt;/h*&gt;</strong>
&lt;table <strong>class="table&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Texte de la légende&lt;/caption&gt;
  &lt;thead&gt;
   &lt;tr&gt;
     <strong>&lt;th scope=&quot;col&quot;&gt;</strong>...&lt;/th&gt;
   &lt;/tr&gt;
  &lt;/thead&gt;
  &lt;tbody&gt;
   &lt;tr&gt;
    &lt;td&gt;...&lt;/td&gt;
   &lt;tr&gt;
  &lt;/tbody&gt;
&lt;/table&gt;
</code><code>
// Cellules vides dans un tableau:
&lt;table <strong>class=&quot;table&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;c&lt;/caption&gt;
&lt;thead&gt;
    &lt;tr&gt;
     &lt;th scope=&quot;col&quot;&gt;...&lt;/th&gt;
     &lt;th scope=&quot;col&quot;&gt;...&lt;/th&gt;
    &lt;/tr&gt;
  &lt;/thead&gt;
  &lt;tbody&gt;
   &lt;tr&gt;
    <strong>&lt;td&gt;-&lt;/td&gt;</strong>
    <strong>&lt;td&gt;-&lt;/td&gt;</strong>
   &lt;tr&gt;
  &lt;/tbody&gt;
&lt;/table&gt;</code><code>

// Légende du tableau :
&lt;table <strong>class=&quot;table&quot;</strong>&gt;
  <strong>&lt;caption&gt;Texte de la légende&lt;/caption&gt;</strong>
    &lt;thead&gt;...&lt;/thead&gt;
    &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h3 id="enhanced">Utilisation avancée</h3>
  <h4 id="width"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-arrows-alt-h fa-stack-1x fa-inverse"></span></span> Modifier la largeur des colonnes et des tableaux</h4>
  <p>Utilisez le <a href="grids-fr.html"><abbr title="feuille de style en cascade">CSS</abbr> de grille</a> pour modifier la largeur des colonnes.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <table class="table">
            <caption class="wb-inv">
            Exemple de tableau avec des colonnes et une largeur modifiées
            </caption>
            <thead>
              <tr>
                <th  scope="col"  class="col-sm-7">En-tête</th>
                <th  scope="col" class="col-sm-5">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Données données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Assurez-vous que la largeur du tableau <code>&lt;table&gt;</code> dans son ensemble, ainsi que celle de chaque colonne <code>&lt;th&gt;</code>, conviennent au contenu
          <ul>
            <li>Les tableaux qui ont trop d'espaces blancs (trop grande séparation) ou trop peu d'espaces blancs (entassement) sont difficiles à lire</li>
          </ul>
        </li>
        <li>Insérez la balise <code>&lt;table&gt;</code> dans un conteneur approprié pour limiter la taille globale du tableau</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cette composante d'une façon qui entre en conflit avec les points de conformité précédent(s) <span class="nowrap"></span></li>
        <li>N'appliquez pas la même largeur à tous les tableaux d'une page simplement pour des raisons de conception</li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code><strong>// </strong>Tableau avec une colonne limitée et une largeur globale<strong>
&lt;div <strong>class=&quot;col-md-3&quot;</strong>&gt;</strong><strong>
</strong> &lt;table <strong>class=&quot;table&quot;</strong>&gt;
 &lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Texte de la légende&lt;/caption&gt;
   &lt;thead&gt;
   &lt;tr&gt;
      &lt;th scope=&quot;col&quot; <strong>class=&quot;col-sm-8&quot;</strong>&gt;...&lt;/th&gt;
      &lt;th scope=&quot;col&quot; <strong>class=&quot;col-sm-4&quot;</strong>&gt;...&lt;/th&gt;
    &lt;/tr&gt;
   &lt;/thead&gt;
   &lt;tbody&gt;
    &lt;tr&gt;
     &lt;td&gt;...&lt;/td&gt;
     &lt;td&gt;...&lt;/td&gt;
    &lt;/tr&gt;
   &lt;/tbody&gt;
 &lt;/table&gt;
&lt;/div&gt;</code>
</pre>
    </div>
  </div>
  <h4 id="striped"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-bars fa-stack-1x fa-inverse"></span></span> Rangées rayées (Zébrures) </h4>
  <p>Les utiliser pour ajouter des rayages du zèbre à n'importe quelle rangée d'un tableau.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <table class="table table-striped">
            <caption class="wb-inv">
            Exemple de tableau avec des rayages du zèbre
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.table-striped</code> dans <code>&lt;tbody&gt;</code> pour mieux distinguer les rangées les unes des autres</li>
        <li>L'utiliser principalement dans les tableaux longs et complexes</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>
&lt;table <strong>class=&quot;table table-striped&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Texte de la légende&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="hover"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-hand-point-up fa-stack-1x fa-inverse"></span></span> Rangées à pointage</h4>
  <p>Les utiliser pour ajouter un effet de pointage appliquant des zébrures à n'importe quelle rangée d'un tableau à l'intérieur de  <code>&lt;tbody&gt;</code>.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <table class="table table-hover">
            <caption class="wb-inv">
            Exemple de tableau avec rangées à pointage
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.table-hover</code> pour permettre à l'utilisateur de mettre chaque rangée en surbrillance lorsqu'il fait glisser son curseur au-dessus</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>
&lt;table <strong>class=&quot;table table-hover&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Texte de la légende&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="bordered"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-table fa-stack-1x fa-inverse"></span></span> Rangées à bordure </h4>
  <p>Les utiliser pour ajouter des bordures au tableau.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <table class="table table-bordered">
            <caption class="wb-inv">
            Exemple de tableau avec des rangées à bordure
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.table-bordered</code> pour séparer des renseignements lorsque les cellules d'un tableau comprennent beaucoup de données, et utilisez le retour automatique à la ligne
          <ul>
            <li>Cela permet à l'utilisateur d'associer facilement les renseignements aux cellules</li>
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
      <pre><code>
&lt;table <strong>class=&quot;table table-bordered&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Texte de la légende&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="condensed"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8615; &#8613;</span></span> Rangées condensées</h4>
  <p>Les utiliser pour réduire le remplissage dans le tableau.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <table class="table table-condensed">
            <caption class="wb-inv">
            Exemple de tableau avec des rangées condensées
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td>Données données</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>Utilisez <code>.table-condensed</code> pour rétrécir la hauteur des rangées</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>
&lt;table <strong>class=&quot;table table-condensed&quot;</strong>&gt;
&lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Texte de la légende&lt;/caption&gt;
  &lt;thead&gt;...&lt;/thead&gt;
  &lt;tbody&gt;...&lt;/tbody&gt;
&lt;/table&gt;</code></pre>
    </div>
  </div>
  <h4 id="responsive"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-mobile-alt fa-stack-1x fa-inverse"></span></span> Tableaux réactifs</h4>
  <p>Créez des tableaux réactifs pour permettre le défilement horizontal de tableaux sur les petits appareils (d'une largeur de moins de 768 px). Lorsque la largeur est supérieure à 768 px, il n'y a aucune différence visuelle dans ces tableaux.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <div class="table-responsive">
            <table class="table">
              <caption class="wb-inv">
              Exemple de tableau avec conception réactive
              </caption>
              <thead>
                <tr>
                  <th scope="col">En-tête</th>
                  <th scope="col">En-tête</th>
                  <th scope="col">En-tête</th>
                  <th scope="col">En-tête</th>
                  <th scope="col">En-tête</th>
                  <th scope="col">En-tête</th>
                  <th scope="col">En-tête</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                </tr>
                <tr>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                </tr>
                <tr>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                  <td>Données données</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>Faites envelopper  <code>.table</code> dans <code>.table-responsive</code> lorsque le tableau est large et nécessite un défilement horizontal sur les appareils mobiles</li>
        <li>Divisez les tableaux volumineux en tableaux plus petits pour rendre le contenu plus convivial</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;div <strong>class=&quot;table-responsive&quot;</strong>&gt;
&lt;table <strong>class=&quot;table&quot;</strong>&gt;
 &lt;caption <strong>class=&quot;wb-inv&quot;</strong>&gt;Texte de la légende&lt;/caption&gt;
    &lt;thead&gt;...&lt;/thead&gt;
    &lt;tbody&gt;...&lt;/tbody&gt;
  &lt;/table&gt;
&lt;/div&gt;</code></pre>
    </div>
  </div>
  <h4 id="colours"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-tint fa-stack-1x fa-inverse"></span></span> Rangées et cellules colorées </h4>
  <p>Utilisez les classes contextuelles pour colorer des rangées de tableau ou des cellules individuelles.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <table class="table">
            <caption class="wb-inv">
            Exemple de tableau avec de la couleur
            </caption>
            <thead>
              <tr>
                <th scope="col">En-tête</th>
                <th scope="col">En-tête</th>
              </tr>
            </thead>
            <tbody>
              <tr class="active">
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td class="active">Données</td>
              </tr>
              <tr class="success">
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td class="success">Données</td>
              </tr>
              <tr class="warning">
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td class="warning">Données</td>
              </tr>
              <tr class="danger">
                <td>Données données</td>
                <td>Données données</td>
              </tr>
              <tr>
                <td>Données données</td>
                <td class="danger">Données</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li><code>.active</code>: Applique la couleur sélectionnée par pointage  à une rangée ou une cellule en particulier</li>
        <li><code>.success</code>:
          Indique une action réussie ou positive</li>
        <li><code>.warning</code>:
          Indique un avertissement qui pourrait exiger une attention particulière</li>
        <li><code>.danger</code>:
          Indique une action dangereuse ou possiblement négative</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>//Dans des rangées :
&lt;tr <strong>class=&quot;active&quot;</strong>&gt;...&lt;/tr&gt;
&lt;tr <strong>class=&quot;success&quot;</strong>&gt;...&lt;/tr&gt;
&lt;tr <strong>class=&quot;warning&quot;</strong>&gt;...&lt;/tr&gt;
&lt;tr <strong>class=&quot;danger&quot;</strong>&gt;...&lt;/tr&gt;

//Dans des cellules de données ou d'en-tête (« td ») ou (« th ») :
&lt;tr&gt;
  &lt;td <strong>class=&quot;active&quot;</strong>&gt;...&lt;/td&gt;
  &lt;td <strong>class=&quot;success&quot;</strong>&gt;...&lt;/td&gt;
  &lt;td <strong>class=&quot;warning&quot;</strong>&gt;...&lt;/td&gt;
  &lt;td <strong>class=&quot;danger&quot;</strong>&gt;...&lt;/td&gt;
&lt;/tr&gt;</code></pre>
    </div>
  </div>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires</h4>
  <p>Des caractéristiques et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/tables/tables-fr.html" >DataTables</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/charts/charts-fr.html" >Graphiques</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/docs/ref/zebra/zebra-fr.html" >Zébrures (technique avancée)</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/demos/tablevalidator/tablevalidator-fr.html" >Validateur de tableau</a></li>
    <li><a class="btn btn-default" href="https://wet-boew.github.io/v4.0-ci/demos/equalheight/equalheight-fr.html" >Égalisation (égalisation des hauteurs)</a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Principes à l'appui</h2>
  <div data-ajax-replace="../writing/strctr-fr.html #tables-info"></div>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
