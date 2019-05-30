---
published: true
layout: default-theme-wet-boew-fr
title: Proximité des marges
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
  <p>L'utiliser pour augmenter ou diminuer la proximité d'un objet par rapport à un autre. Cela vient modifier les espaces blancs entre deux éléments afin d'indiquer si les éléments sont liés ou non. De plus, ces classes permettent à des éléments de contenu figurant dans une grille et ne figurant pas dans une grille d'exister dans la même rangée. </p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base</h3>
  <div class="row">
    <div class="col-sm-6 col-lg-3">
      <h4 id="top"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8613; </span></span> Marge du haut</h4>
      <p>Élargir ou rétrécir la marge du haut par défaut d'un élément (en-tête, tableau, liste) ou d'un objet de conception (panneau, classe « well », grille...)</p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Détails</h5>
          <ul>
            <li><code>.mrgn-tp-0</code> = 0px</li>
            <li><code>.mrgn-tp-sm</code> = 5px</li>
            <li><code>.mrgn-tp-md</code> = 15px</li>
            <li><code>.mrgn-tp-lg</code> = 30px</li>
            <li><code>.mrgn-tp-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-sm-6 col-lg-3">
      <h4 id="bottom"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8615; </span></span> Marge du bas</h4>
      <p>Élargir ou rétrécir la marge du bas par défaut d'un élément (en-tête, tableau, liste) ou d'un objet de conception (panneau, classe « well », grille...) </p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Détails</h5>
          <ul>
            <li><code>.mrgn-bttm-0</code> = 0px</li>
            <li><code>.mrgn-bttm-sm</code> = 5px</li>
            <li><code>.mrgn-bttm-md</code> = 15px</li>
            <li><code>.mrgn-bttm-lg</code> = 30px</li>
            <li><code>.mrgn-bttm-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
  <div class="clear visible-md"></div>
    <div class="col-sm-6 col-lg-3">
      <h4 id="left"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8612; </span></span> Marge de gauche</h4>
      <p>Élargir ou rétrécir la marge de gauche par défaut d'un élément (en-tête, tableau, liste) ou d'un objet de conception (panneau, classe « well », grille...) </p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Détails</h5>
          <ul>
            <li><code>.mrgn-lft-0</code> = 0px</li>
            <li><code>.mrgn-lft-sm</code> = 5px</li>
            <li><code>.mrgn-lft-md</code> = 15px</li>
            <li><code>.mrgn-lft-lg</code> = 30px</li>
            <li><code>.mrgn-lft-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-sm-6 col-lg-3">
      <h4 id="right"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-inverse">&#8614; </span></span> Marge de droite</h4>
      <p>Élargir ou rétrécir la marge de droite par défaut d'un élément (en-tête, tableau, liste) ou d'un objet de conception (panneau, classe « well », grille...) </p>
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Détails</h5>
          <ul>
            <li><code>.mrgn-rght-0</code> = 0px</li>
            <li><code>.mrgn-rght-sm</code> = 5px</li>
            <li><code>.mrgn-rght-md</code> = 15px</li>
            <li><code>.mrgn-rght-lg</code> = 30px</li>
            <li><code>.mrgn-rght-xl</code> = 50px</li>
          </ul>
        </div>
      </div>
    </div>
  </div>

          <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
<p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
            <li>L'utiliser pour élargir ou rétrécir l'espace blanc entre des objets</li>
			<li>Comprenez et mettez en œuvre les <a href="#supporting"> principes à l'appui</a> connexes</li>
          </ul>

          <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5><p><span class="nowrap">Point d'observation&nbsp;:</span></p><ul>
          <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
        </ul>

  <h3 id="enhanced">Utilisation améliorée</h3><h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires</h4> <p>Des caractéristiques et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="reflow-fr.html">Redistribution du contenu autour de grilles</a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Principes à l'appui</h2>
  <p>L'augmentation ou la diminution de la proximité et de l'espace blanc indique que soit des éléments de contenu sont associés, soit ils ne sont pas liés.</p>
  <blockquote>
    <p>[Traduction] En perception visuelle, le principe de la proximité est très simple : les choses qui sont spatialement rapprochées les unes des autres sont considérées comme liées. Nous pouvons utiliser ce principe pour indiquer clairement lorsque des éléments [...] sont associés et lorsqu'ils sont séparés.</p>
    <p>Rapprochez les choses qui sont liées et distancez les choses qui doivent être considérées comme séparées.</p>
    <p>Nous pouvons appliquer le principe de la proximité à l'envers : les éléments qui sont distancés les uns des autres sont considérés comme séparés. </p>
     <footer class="text-right">Formulate Information Design<br>
      <cite><a href="https://www.formulate.com.au/blog/perception-5-proximity" >Perception and the design of forms — Part 5: Proximity</a></cite></footer>
  </blockquote>
  <blockquote>
    <p>[Traduction] Le principe de la proximité nécessite que les éléments liés soient groupés visuellement, ce qui crée moins d'encombrement et qui offre une mise en page plus organisée. Les éléments qui ne sont pas liés les uns aux autres devraient être plus éloignés les uns des autres pour souligner leur absence de relation.</p>
    <p>Une utilisation efficace des espaces blancs et le groupement des éléments liés sont essentiels afin d'appliquer à votre site Web une hiérarchie visuelle claire.</p>
    <footer class="text-right">Louis Lazaris<br>
      <cite><a href="https://www.webdesignerdepot.com/2010/01/the-principle-of-proximity-in-web-design/" >The Principle of Proximity in Web Design </a></cite></footer>
  </blockquote>
{% endraw %}
{:/}
