---
published: true
layout: default-theme-wet-boew-fr
title: Alignement
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
                    <li><a href="#left">Texte aligné à gauche</a></li>
                    <li><a href="#centre">Texte aligné au centre</a></li>
                    <li><a href="#centre-bl">Blocs de contenu au centre</a></li>
                    <li><a href="#right">Texte aligné à droite  </a></li>
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
          <h2 class="mrgn-tp-0 h4 text-warning"><span class="fa fa-exclamation-triangle"></span> Travail en cours</h2>
          <p>Cette page est un travail en cours.</p>
          <p>Veuillez <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">présenter une question</a> ou envoyer une demande d'extraction si des renseignements ou des codes sont manquants, inexacts ou décalés par rapport au référentiel principal (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <section>
    <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage </h2>
    <p>Utilisez cette fonction pour aligner le texte à gauche, au centre ou à droite. Sinon, utilisez-la pour aligner un bloc de contenu ou une image au centre.</p>
  </section>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage </h2>
  <h3 id="basic">Utilisation de base</h3>
  <h4 id="left"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-left fa-stack-1x fa-inverse"></span></span> Texte aligné à gauche</h4>
  <p>Utilisez cette fonction pour aligner le texte à gauche.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-left">(Le contenu est indiqué ici)</p>

        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>Appliquez <code>.text-left</code> à un élément pour aligner à gauche le texte qu'il contient</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
        <li>N'utilisez pas cette fonction pour aligner des renseignements non textuels</li>
      </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p <strong>class=&quot;text-left&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="centre"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-center fa-stack-1x fa-inverse"></span></span> Texte aligné au centre</h4>
  <p>Utilisez cette fonction pour aligner le texte au centre.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-center">(Le contenu est indiqué ici)</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Appliquez <code>.text-center</code> à un élément pour aligner au centre le texte qu'il contient</li>
		<li>Appliquez au besoin, aux cellules de données d'un tableau afin d'imiter des tableaux comptables</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>

		<li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Évitez cet élément, sauf s'il ajoute de la valeur au contenu.<br>
          <blockquote>
            <p>Les textes alignés au centre et à droite présentent sont tous deux « décalés » à gauche, ce qui a été démontré nuire à la vitesse de lecture et à la compréhension. La combinaison d'une bordure gauche droite (ou « nette ») et d'une bordure droite décalée du texte aligné à gauche standard est ce qui fonctionne le mieux pour les lecteurs, car cela aide l'oeil à trouver le début de la prochaine ligne lorsqu'il quitte la fin de la dernière ligne.</p>
		    <footer class="text-right"><a href="https://mrwweb.com/no-justification-dont-use-right-center-and-full-justification-on-the-web/" >No Justification: Don’t Use Right, Center, and Full Justification on the Web (en anglais seulement)</a></footer>
	      (Aucune justification : n'utilisez pas la justification à droite, au centre ou complète dans le Web)</blockquote>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p <strong>class=&quot;text-center&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="centre-bl"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-center fa-stack-1x fa-inverse"></span></span> Centrer des blocs de contenu</h4>
  <p>Utilisez cette fonction afin de centrer un bloc dans son ensemble, y compris le texte. Centrer un bloc prend un élément dont la largeur est fixe, et applique une marge gauche et une marge droite égales, ce qui centre le contenu.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <img src="https://placehold.it/140x140" class="img-rounded center-block" alt="Une image de paramètre fictif carré dont les coins sont arrondis" /></div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
        <li>Appliquer <code>.center-block</code> à un bloc d'éléments dont la largeur est fixe pour l'aligner au centre</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec le point d'observation précédent</li>
        <li>Évitez cet élément, sauf s'il ajoute de la valeur au contenu.<br>
          <blockquote>
            <p>Les textes alignés au centre et à droite présentent sont tous deux « décalés » à gauche, ce qui a été démontré nuire à la vitesse de lecture et à la compréhension. La combinaison d'une bordure gauche droite (ou « nette ») et d'une bordure droite décalée du texte aligné à gauche standard est ce qui fonctionne le mieux pour les lecteurs, car cela aide l'oeil à trouver le début de la prochaine ligne lorsqu'il quitte la fin de la dernière ligne.</p>
            <footer class="text-right"><a href="https://mrwweb.com/no-justification-dont-use-right-center-and-full-justification-on-the-web/" ><span lang="en">No Justification: Don’t Use Right, Center, and Full Justification on the Web</span> (en anglais seulement)</a></footer>
          </blockquote>
        </li>
        </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;img <strong>class=&quot;center-block&quot;</strong> alt=&quot;...&quot; src=&quot;x.jpg&quot; /&gt;</code></pre>
    </div>
  </div>
  <h4 id="right"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-align-right fa-stack-1x fa-inverse"></span></span> Texte aligné à droite</h4>
  <p>Utilisez cette fonction pour aligner le texte à droite.</p>
  <div class="row">
    <div class="col-md-3">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p class="text-right">(Le contenu est indiqué ici)</p>
        </div>
      </div>
    </div>
    <div class="col-md-5">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
        <li>Appliquez <code>.text-right</code> à un élément pour aligner à droite le texte qu'il contient</li>
		<li>Appliquez cette fonction, au besoin, aux cellules de données d'un tableau afin d'imiter des tableaux comptables</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>Évitez cet élément, sauf s'il ajoute de la valeur au contenu.
          <blockquote>
            <p>Les textes alignés au centre et à droite présentent sont tous deux « décalés » à gauche, ce qui a été démontré nuire à la vitesse de lecture et à la compréhension. La combinaison d'une bordure gauche droite (ou « nette ») et d'une bordure droite décalée du texte aligné à gauche standard est ce qui fonctionne le mieux pour les lecteurs, car cela aide l'oeil à trouver le début de la prochaine ligne lorsqu'il quitte la fin de la dernière ligne.</p>
            <footer class="text-right"><a href="https://mrwweb.com/no-justification-dont-use-right-center-and-full-justification-on-the-web/" ><span lang="en">No Justification: Don’t Use Right, Center, and Full Justification on the Web</span> (en anglais seulement)</a></footer>
          </blockquote>
        </li>
       </ul>
    </div>
    <div class="col-md-4">
	<h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p <strong>class=&quot;text-right&quot;</strong>&gt;...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page provient de <a href="https://getbootstrap.com/" rel="external">Bootstrap<span  class="wb-inv"> (lien externe)</span></a></p>
{% endraw %}
{:/}
