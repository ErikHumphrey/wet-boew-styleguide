---
published: true
layout: default-theme-wet-boew-fr
title: Liens
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
                <li><a href="#basic">Utilisation de base </a></li>
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
          <h2 class="mrgn-tp-0 h4 text-warning"><span class="fa fa-exclamation-triangle"></span> Chantier</h2>
          <p>Cette  page est en chantier.</p>
          <p>Veuillez <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème </a>  ou soumettre une demande de tirage si des renseignements ou des codes sont manquants, incorrects ou que leur synchronisation est déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <section>
    <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage </h2>
    <p>Utilisez un lien  (texte et/ou  image) pour faire passer un utilisateur à une autre page Web, à un autre endroit sur la même page Web ou pour exécuter une fonction de contrôle de l'utilisateur déterminé par un script du côté du client (JavaScript). </p>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
    <h3 id="basic">Utilisation de base </h3>
    <h4 id="default"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-cogs fa-stack-1x fa-inverse"></span></span> Défaut </h4>
    <p>Utiliser un mot, une expression ou une  image qui permet à l'utilisateur d'interagir avec le contenu sur un écran, ce qui peut prendre la forme d'une navigation, d'une interrogation ou d'une  interaction avec le contenu.</p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0 h5">Apparence</h5>
            <p><a href="#">Lien par défaut</a></p>
            <p class="mrgn-bttm-0"><a href="#">Lien et image liée.<img class="img-thumbnail left-block" alt="A generic square placeholder image with a white border around it" src="https://placehold.it/100x100"></a></p>
          </div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>Utilisez-les pour relier une page à une autre</li>
          <li>Utilisez-les pour faire un lien vers une section sur une  page</li>
          <li>Utilisez-les pour ouvrir un <a href="https://wet-boew.github.io/wet-boew/demos/overlay/overlay-fr.html" >contenu superposé</a> ou une <a href="https://wet-boew.github.io/wet-boew/demos/lightbox/lightbox-fr.html" >boîte de dialogue modale ou la lightbox</a></li>
          <li>Utilisez-les pour lancer un événement ou une interrogation</li>
          <li>Utilisez-les pour ouvrir un nouveau message de courriel sortant</li>
          <li>Comprenez et mettez en place les <a href="#supporting">principes de soutien </a>connexes</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
        <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
          <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité  précédents</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>// Lien par défaut&nbsp;:
<strong>&lt;a href=&quot;#&quot;&gt;</strong>...&lt;/a&gt;

// Lien et image liée&nbsp;:
<strong>&lt;a href=&quot;#&quot;&gt;&lt;img src=&quot;#&quot;</strong> alt=&quot;&quot; /&gt;&lt;/a&gt;</code></pre>
      </div>
    </div>
  </section>
  <h3 id="enhanced">Utilisation améliorée</h3>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires </h4>
  <p>Des fonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a href="buttons-fr.html" class="btn btn-default">Boutons</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-fr.html"  class="btn btn-default">Carrousel</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/details/details-fr.html"   class="btn btn-default">Agrandir et dissimuler « affichable/masquable » </a></li>
    <li><a href="listgroup-fr.html" class="btn btn-default">List group </a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/lightbox/lightbox-fr.html"  class="btn btn-default">Fenêtre modale (lightbox)</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/overlay/overlay-fr.html"  class="btn btn-default">Contenu superposé  </a></li>
    <li><a href="pagination-fr.html" class="btn btn-default">Pagination</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/tabs/tabs-fr.html"  class="btn btn-default">Onglets</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/toggle/toggle-fr.html" class="btn btn-default">Basculer</a></li>
    <li><a href="https://wet-boew.github.io/v4.0-ci/docs/ref/lightbox/lightbox-fr.html"  class="btn btn-default">Galerie de miniatures et de photos (lightbox) </a></li>
  </ul>
  <h2 id="supporting"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span> </span> Principes de soutien </h2>
  <h3><span data-ajax-replace="../writing/strctr-fr.html #links-heading"></span></h3>
  <div data-ajax-replace="../writing/strctr-fr.html #links-info"></div>
  <h3><span data-ajax-replace="../writing/stl-fr.html #scent-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-fr.html #scent-info"></div>
  <h3><span data-ajax-replace="../writing/stl-fr.html #parallel-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-fr.html #parallel-info"></div>
  <h3><span data-ajax-replace="../writing/stl-fr.html #scan-heading"></span></h3>
  <div data-ajax-replace="../writing/stl-fr.html #scan-info"></div>
  <h3><span data-ajax-replace="../writing/rchtctr-fr.html #alphabetization-heading"></span></h3>
  <div data-ajax-replace="../writing/rchtctr-fr.html #alphabetization-info"></div>
  <p class="mrgn-tp-lg text-muted">Remarque&nbsp;: Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
