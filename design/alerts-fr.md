---
published: true
layout: default-theme-wet-boew-fr
title: Alertes
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
                    <li><a href="#links">Liens d'alertes</a></li>
                    <li><a href="#addon">Fonctions complémentaires</a></li>
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
    <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage</h2>
    <p>Utilisez cette fonction afin de fournir des messages de rétroaction contextuels pour les mesures habituelles prises par les utilisateurs. Faites un choix à partir d'une poignée de messages d'alertes disponibles et souples.</p>
  </section>
  <section>
    <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage </h2>
    <h3 id="basic">Utilisation de base </h3>
    <p>Utilisez cette fonction pour boucler tout texte et un bouton ignorer facultatif dans <code>.alert</code>, ou dans l'une des quatre catégories contextuelles (par exemple, <code>.alert-success</code>) pour les messages d'alertes de base.</p>
    <p>Les alertes n'appartiennent pas à une catégorie par défaut, seulement des catégories de base et de modificateur. Une alerte grise par défaut n'a pas beaucoup de sens, par conséquent, précisez toujours un type d'alerte au moyen d'une catégorie contextuelle. Choisissez parmi réussite, information, avertissement ou danger.</p>
    <h4 id="success"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-check fa-stack-1x fa-inverse"></span></span> Alerte de réussite</h4>
    <p>Utilisez cette alerte pour attirer l'attention sur des renseignements qui doivent se distinguer du reste du contenu de la page. Avec l'alerte de réussite, le titre apparaît à côté d'une coche; l'arrière-plan du contenu est vert.</p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Apparence</h5>
            <h6>Alerte comprenant un en-tête</h6>
            <section class="alert alert-success">
              <h3>(Titre)</h3>
              <p>(Le contenu de la réussite est indiqué ici.)</p>
            </section>

<h6>Alerte sans en-tête</h6>
<p>(Le contenu régulier est indiqué ici.)</p>
 <div class="alert alert-success">
<p>(Le contenu de la réussite est indiqué ici.)</p>
 </div>
          </div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
        <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
        <ul>
          <li>Utilisez <code>.alert-success</code> <strong>pour reconnaître quelque chose de positif</strong>; par exemple, une tâche achevée, quelque chose d'exact</li>
          <li>Placez-la dans le flux logique d'une page</li>
          <li>Assurez-vous qu'elle est liée au contenu qui l'entoure immédiatement</li>
          <li>Commencez la balise <code>&lt;section&gt;</code> par un en-tête qui est propre au contenu présenté et qui est contenu à l'intérieur de celui-ci</li>
          <li> Utilisez un en-tête général uniquement si un en-tête particulier n'est pas possible (par exemple, « Félicitations »)</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
          <li>N'utilisez pas la balise <code>&lt;section&gt;</code> à l'intérieur d'une autre section, cela cause des problèmes de validation
            <ul>
              <li>Utiliser la balise <code>&lt;div&gt;</code> pour styliser l'alerte</li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>// Alerte avec un en-tête
&lt;section <strong>class=&quot;alert alert-success&quot;</strong>&gt;
<strong>  &lt;h*&gt;...&lt;/h*&gt;</strong>
  ...
&lt;/section&gt;

// Alerte sans en-tête
&lt;div <strong>class=&quot;alert alert-success&quot;</strong>&gt;
   &lt;p&gt;...&lt;/p&gt;
&lt;/div&gt;</code></pre>
      </div>
    </div>
    <h4 id="info"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Alerte d'information</h4>
    <p>Utilisez cette fonction pour mettre en évidence des renseignements ciblés pour des groupes de segments précis. Avec l'alerte d'information, le titre apparaît à côté d'une icône de la lettre « i »; l'arrière-plan du contenu est bleu. Utilisez cette alerte pour attirer l'attention sur des renseignements notables qui doivent se distinguer du reste du contenu de la page. </p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Apparence</h5>
            <h6>Alerte avec un en-tête</h6>
            <section class="alert alert-info">
              <h3>(Titre)</h3>
              <p>(Le contenu de l'alerte d'information est indiqué ici.)</p>
            </section>


<h6>Alerte sans en-tête</h6>
<p>(Le contenu régulier est indiqué ici.)</p>
 <div class="alert alert-info">
<p>(Le contenu de l'alerte d'information est indiqué ici.)</p>
 </div>
          </div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>Utilisez <code>.alert-info</code> <strong>pour mettre en évidence des renseignements passablement importants</strong></li>
          <li>Placez-la dans le flux logique d'une page</li>
          <li>Assurez-vous qu'elle est liée au contenu qui l'entoure immédiatement</li>
          <li>Commencez la balise <code>&lt;section&gt;</code> par un en-tête qui est propre au contenu présenté et contenu à l'intérieur de celui-ci</li>
          <li>Utilisez un en-tête général seulement si un en-tête précis n'est pas possible (par exemple, « Conseil », « Résumé », « Remarque »)</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
          <li>N'utilisez pas la balise <code>&lt;section&gt;</code> à l'intérieur d'une autre section, cela cause des problèmes de validation
            <ul>
                <li>Utiliser la balise <code>&lt;div&gt;</code> pour styliser l'alerte</li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>// Alerte avec un en-tête
&lt;section <strong>class=&quot;alert alert-info&quot;</strong>&gt;
<strong>  &lt;h*&gt;...&lt;/h*&gt;</strong>
  ...
&lt;/section&gt;

// Alerte sans en-tête
&lt;div <strong>class=&quot;alert alert-info&quot;</strong>&gt;
   &lt;p&gt;...&lt;/p&gt;
&lt;/div&gt;
</code></pre>
      </div>
    </div>
    <h4 id="warning"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-triangle fa-stack-1x fa-inverse"></span></span> Alerte d'avertissement </h4>
    <p>Utilisez cette alerte pour attirer l'attention sur des renseignements qui doivent se distinguer du reste du contenu de la page.  Avec l'alerte d'avertissement, le titre apparaît à côté d'une icône de mise en garde; l'arrière-plan du contenu est jaune. </p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Apparence</h5>
            <h6>Alerte avec un en-tête</h6>
            <section class="alert alert-warning">
              <h3>(Titre)</h3>
              <p>(Le contenu de l'avertissement est indiqué ici.)</p>
            </section>


<h6>Alerte sans en-tête</h6>
<p>(Le contenu régulier est indiqué ici.)</p>
 <div class="alert alert-warning">
<p>(Le contenu de l'avertissement est indiqué ici.)</p>
 </div>
          </div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>Utilisez <code>.alert-warning</code> <strong>pour avertir l'utilisateur</strong></li>
          <li>Placez-la dans le flux logique d'une page</li>
          <li>Assurez-vous qu'elle est liée au contenu qui l'entoure immédiatement</li>
          <li>Commencez la balise <code>&lt;section&gt;</code> par un en-tête qui est propre au contenu présenté et qui est contenu à l'intérieur de celui-ci</li>
          <li>Utilisez un en-tête général uniquement si un en-tête précis n'est pas possible (par exemple, « Avertissement », « Alerte »)</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation </h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
          <li>N'utilisez pas la balise <code>&lt;section&gt;</code> à l'intérieur d'une autre section, cela cause des problèmes de validation
            <ul>
                <li>Utiliser la balise <code>&lt;div&gt;</code> pour styliser l'alerte</li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>// Alerte avec un en-tête<strong>
</strong>&lt;section <strong>class=&quot;alert alert-warning&quot;</strong>&gt;
<strong>  &lt;h*&gt;...&lt;/h*&gt;</strong>
  ...
&lt;/section&gt;

// Alerte sans en-tête
&lt;div <strong>class=&quot;alert alert-warning&quot;</strong>&gt;
   &lt;p&gt;...&lt;/p&gt;
&lt;/div&gt;
</code></pre>
      </div>
    </div>
    <h4 id="danger"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-exclamation-circle fa-stack-1x fa-inverse"></span></span> Alerte de danger</h4>
    <p>Utilisez cette alerte pour attirer l'attention sur des renseignements qui doivent se distinguer du reste du contenu de la page. Avec l'alerte de danger, le titre apparaît à côté d'une icône de point d'exclamation; l'arrière-plan du contenu est rouge. </p>
    <div class="row">
      <div class="col-md-3">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Apparence</h5>
            <h6>Alerte avec un en-tête</h6>
            <section class="alert alert-danger">
              <h3>(Titre)</h3>
              <p>(Le contenu de l'alerte de danger est indiqué ici.)</p>
            </section>


<h6>Alerte sans en-tête</h6>
<p>(Le contenu régulier est indiqué ici.)</p>
 <div class="alert alert-danger">
<p>(Le contenu de l'alerte de danger est indiqué ici.)</p>
 </div>
          </div>
        </div>
      </div>
      <div class="col-md-5">
        <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation </h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>Utilisez <code>.alert-danger</code><strong> pour les mesures ou les renseignements très importants, négatifs ou dangereux</strong>, par exemple, les systèmes sont en panne,
            modifications à X en attente, « Êtes-vous sûr que vous voulez supprimer X? » </li>
          <li>Placez dans le flux logique d'une page</li>
          <li>Assurez-vous qu'il est lié au contenu qui l'entoure immédiatement</li>
          <li>Commencez la balise <code>&lt;section&gt;</code> par un en-tête qui est propre au contenu présenté et qui est contenu à l'intérieur de celui-ci</li>
          <li>Utilisez un en-tête général uniquement si un en-tête précis n'est pas possible (par exemple, « Avertissement important », « Attention »)</li>
        </ul>
        <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
        <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
        <ul>
          <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec les points de conformité précédents</li>
          <li>N'utilisez pas la balise <code>&lt;section&gt;</code> à l'intérieur d'une autre section, cela cause des problèmes de validation
            <ul>
                <li>Utiliser la balise <code>&lt;div&gt;</code> pour styliser l'alerte</li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mrgn-tp-0">Code</h5>
        <pre><code>// Alerte avec un en-tête<strong>
</strong>&lt;section <strong>class=&quot;alert alert-danger&quot;</strong>&gt;
<strong>  &lt;h*&gt;...&lt;/h*&gt;</strong>
  ...
&lt;/section&gt;

// Alerte sans en-tête
&lt;div <strong>class=&quot;alert alert-danger&quot;</strong>&gt;
    &lt;p&gt;...&lt;/p&gt;
&lt;/div&gt;
</code></pre>
      </div>
    </div>
  </section>
  <section>
    <h3 id="enhanced">Utilisation améliorée</h3>
    <h4 id="links"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-link fa-stack-1x fa-inverse"></span></span> Liens d'alerte </h4>
    <p>Utilisez cette fonction pour contourner l'apparence par défaut d'un lien, utilisez la catégorie utilitaire <code>.alert-link</code> afin de fournir rapidement des liens colorés correspondant dans toute alerte.</p>
    <div class="row">
      <div class="col-md-4">
        <div class="panel panel-default">
          <div class="panel-body">
            <h5 class="mrgn-tp-0">Apparence</h5>
            <section class="alert alert-success">
              <h3>(Titre)</h3>
              <p>(Le contenu de l'alerte de réussite est indiqué ici <a href="#" class="alert-link">texte du lien</a>.)</p>
            </section>
            <section class="alert alert-info">
              <h3>(Titre)</h3>
              <p>(Le contenu de l'alerte d'information est indiqué ici <a href="#" class="alert-link">texte du lien</a>.)</p>
            </section>
            <section class="alert alert-warning">
              <h3>(Titre)</h3>
              <p>(Le contenu de l'alerte avertissement est indiqué ici <a href="#" class="alert-link">texte du lien</a>.)</p>
            </section>
            <section class="alert alert-danger">
              <h3>(Titre)</h3>
              <p>(Le contenu de l'alerte de danger est indiqué ici <a href="#" class="alert-link">texte du lien</a>.)</p>
            </section>
          </div>
        </div>
      </div>
      <div class="col-md-8">
        <h5 class="mrgn-tp-md">Code</h5>
        <pre><code>&lt;section <strong>class=&quot;alert alert-success&quot;</strong>&gt;
  &lt;p&gt;... &lt;a href=&quot;#&quot; <strong>class=&quot;alert-link&quot;</strong>&gt;texte du lien&lt;/a&gt;.&lt;/p&gt;
&lt;/section&gt;

&lt;section <strong>class=&quot;alert alert-info&quot;</strong>&gt;
  &lt;p&gt;... &lt;a href=&quot;#&quot; <strong>class=&quot;alert-link&quot;</strong>&gt;texte du lien&lt;/a&gt;.&lt;/p&gt;
&lt;/section&gt;

&lt;section <strong>class=&quot;alert alert-warning&quot;</strong>&gt;
 &lt;p&gt;... &lt;a href=&quot;#&quot; <strong>class=&quot;alert-link&quot;</strong>&gt;texte du lien&lt;/a&gt;.&lt;/p&gt;
&lt;/section&gt;

&lt;section <strong>class=&quot;alert alert-danger&quot;</strong>&gt;
  &lt;p&gt;... &lt;a href=&quot;#&quot; <strong>class=&quot;alert-link&quot;</strong>&gt;texte du lien&lt;/a&gt;.&lt;/p&gt;
&lt;/section&gt;</code></pre>
      </div>
    </div>
  </section>
  <h4 id="addon"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-stack-1x fa-plus fa-inverse"></span></span> Fonctions complémentaires </h4>
  <p>Des fonctions complémentaires et des comportements supplémentaires sont disponibles.</p>
  <ul class="list-inline lst-spcd">
    <li><a href="https://wet-boew.github.io/v4.0-ci/demos/equalheight/equalheight-fr.html" class="btn btn-default">Égaliser (hauteur égale)</a></li>
  </ul>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page provient de <a href="https://getbootstrap.com/" rel="external">Bootstrap<span class="wb-inv"> (lien externe)</span></a></p>
{% endraw %}
{:/}
