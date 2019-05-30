---
published: true
layout: default-theme-wet-boew-fr
title: Icônes
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
            <li><a href="#des">Conception et codage</a>
              <ul>
                <li><a href="#gly"><span lang="en">Glyphicons</span></a></li>
                <li><a href="#fon">Icônes de police <span lang="en">Font Awesome</span></a></li>
              </ul>
            </li>
            <li><a href="#enh">Utilisation améliorée</a>
              <ul>
                <li><a href="#add">Fonction complémentaires </a> </li>
              </ul>
            </li>
            <li><a href="#sup">Principes de soutien </a></li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
  <h2 id="des"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <p>Utilisez l'un des deux ensembles d'icônes, les <span lang="en">Glyphicons</span> ou la police <span lang="en">Font Awesome</span> à des fins décoratives. Les icônes sont des glyphes − un dessin sur des polices, semblable à la police Wingdings. Il ne transmettent pas de signification, contrairement aux polices traditionnelles. Par conséquent, le texte réel doit accompagner l'icône afin de s'assurer que les exigences en matière d'accessibilité sont respectées. Rendez le texte visible ou invisible, pourvu qu'il soit présent.</p>
  <div class="row wb-eqht mrgn-tp-md">
    <section class="col-md-5">
      <h2 class="mrgn-tp-0 text-success h4"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h2>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>Accompagnez toutes les icônes de texte
          <ul>
            <li>Le texte peut être invisible (<code>.wb-inv</code>) au besoin, mais doit être présent pour des raisons d'accessibilité</li>
          </ul>
        </li>
        <li>Insérez un espace entre la balise <code>&lt;/span&gt;</code> et le texte de lien
              <ul>
            <li>Cela permet d'ajouter un espacement approprié pour que le lien soit facile à lire, par exemple <code>&lt;/span<strong>&gt; texte</strong> du lien&lt;/a&gt;</code></li>
          </ul>
        </li>
        <li>Utilisez les icônes dans une balise <code>&lt;span&gt;</code> lorsqu'elles se trouvent dans un hyperlien (<code>&lt;<strong>a href=""</strong>&gt;&lt;<strong>span class=""</strong>&gt;&lt;<strong>/span</strong>&gt; texte du lien<strong>&lt;/a</strong>&gt;</code></li>
        <li>Comprenez et mettez en place les <a href="#sup">principes de soutien</a> connexe</li>
      </ul>
    </section>
    <section class="col-md-7 brdr-lft">
      <h2 class="mrgn-tp-0 text-danger h4"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h2>
      <p>Points de conformité&nbsp;:</p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
        <li>N'utilisez pas d'icônes pour représenter le logo d'un tiers, car cela est contraire à la politique sur l'image de marque de l'entreprise. Par exemple&nbsp;:
          <ul>
            <li><a href="https://www.facebookbrand.com/dos-donts">Ce qui est acceptable et ce qui ne l'est pas – Facebook</a>&nbsp;: «&nbsp;Utiliser des icônes, images ou marques commerciales pour représenter Facebook, autres que celles qui se trouvent dans ce centre des ressources&nbsp;»</li>
            <li><a href="https://about.twitter.com/press/brand-assets">Lignes directrices et image de marque de Twitter</a> : [Traduction] «&nbsp;Notre logo est toujours bleu ou blanc. L'oiseau de Twitter n'est jamais présenté en noir ou en d'autres couleurs.&nbsp;»</li>
            <li>L'espacement du pixel parfait  et d'autres considérations sont aussi requis. Il est préférable, sur le plan juridique, d'utiliser l'image du logo du tiers</li>
          </ul>
        </li>
      </ul>
    </section>
  </div>
  <h3 id="gly"><span lang="en">Glyphicons</span></h3>
  <p>Les <span lang="en">Glyphicons</span> donnent 250 glyphes. Elles font partie de la version de base de la <abbr title="Boîte à outils de l'expérience Web">BOEW</abbr>. </p>
  <p><a href="https://bootstrapdocs.com/v3.3.1/docs/components/#glyphicons" class="btn btn-primary">Afficher les <span lang="en">Glyphicons</span></a></p>
  <h3 id="fon">Icônes de police <span lang="en">Font Awesome</span> </h3>
  <p>La police <span lang="en">Font Awesome</span> contient plus de 600 glyphes. Ces icônes <strong>ne font pas</strong> partie de   la version de base de la <abbr title="Boîte à outils de l'expérience Web">BOEW</abbr>. Consulter le site web de <a href="https://fontawesome.com/start" lang="en">Font Awesome</a> pour les instructions d'implémentation.</p>
  <p><a href="https://fortawesome.github.io/Font-Awesome/icons/" class="btn btn-primary">Afficher les icônes de police <span lang="en">Font Awesome</span></a> <a href="https://fortawesome.github.io/Font-Awesome/examples/"  class="btn btn-primary">Afficher des exemples d'icône de police <span lang="en">Font Awesome</span> – Empiler, redimensionner, pivoter, tourner </a></p>
  <h2 id="enh">Utilisation améliorée</h2>
  <h3 id="add"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires</h3>
  <p>Des fonctions et des comportements complémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a class="btn btn-default" href="colour-fr.html">Couleur</a></li>
  </ul>
  <h2 id="sup"><span class="fa-stack"> <span class="fa fa-circle fa-stack-2x"></span> <span class="fa fa-bookmark fa-stack-1x fa-inverse"></span></span> Principes de soutien</h2>
  <div data-ajax-replace="../writing/strctr-fr.html #image-info"></div>
{% endraw %}
{:/}
