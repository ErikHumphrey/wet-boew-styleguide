---
published: true
layout: default-theme-wet-boew-fr
title: Effets d'édition de texte
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
            <li> <a href="#design">Conception et codage</a>
              <ul>
                <li> <a href="#basic">Utilisation de base</a>
                  <ul>
                    <li><a href="#marked">Texte marqué</a></li>
                    <li> <a href="#deleted">Texte supprimé</a> </li>
                    <li><a href="#strikethrough">Texte barré</a></li>
                    <li><a href="#inserted">Texte inséré</a></li>
                    <li><a href="#underlined">Texte souligné</a></li>
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
          <p>Veuillez <a href="https://github.com/wet-boew/wet-boew-styleguide/issues/new">transmettre un problème</a> ou soumettre une demande de tirage s'il manque des renseignements ou des codes ou si la synchronisation est incorrecte ou déphasée avec le principal référentiel (wet-boew/wet-boew).</p>
        </div>
      </div>
    </section>
  </div>
  <h2 id="purpose"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-info fa-stack-1x fa-inverse"></span></span> Usage</h2>
  <p>On les utilise pour indiquer les éditions de texte sur une page.</p>
  <h2 id="design"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-paint-brush fa-stack-1x fa-inverse"></span></span> Conception et codage</h2>
  <h3 id="basic">Utilisation de base</h3>
  <h4 id="marked"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="far fa-edit fa-stack-1x fa-inverse"></span></span> Texte marqué</h4>
  <p>L'utiliser pour mettre en surbrillance une section du texte à titre de référence en raison de sa pertinente dans un autre contexte.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Texte ordinaire et
            <mark>texte marqué</mark>
            .</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>L'utiliser pour marquer des renseignements qui  <strong>sont importants dans un autre contexte</strong></li>
        <li>Met du texte en surbrillance pour montrer des termes de recherche correspondants ou pour montrer du texte par rapport à autre chose</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
        <li>Ne l'utilisez pas au lieu du texte gras  (<code>&lt;strong&gt;</code>)
          <ul>
            <li>Cette balise <strong>n</strong>'est <strong>pas</strong> destinée au simple fait de mettre en surbrillance des mots clés, des expressions, des nombres ou des totaux</li>
          </ul>
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;mark&gt;...&lt;/mark&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="deleted"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fas fa-trash-alt fa-stack-1x fa-inverse"></span></span> Texte supprimé</h4>
  <p>L'utiliser pour indiquer que du texte a été supprimé.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Texte ordinaire et <del>texte supprimé</del>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>L'utiliser pour montrer du <strong>texte supprimé récemment</strong></li>
        <li>L'utiliser avec modération, puisqu'l rend une page difficile à lire</li>
        <li>L'utiliser pour montrer  les modifications enregistrées dans un document officiel, comme un procès-verbal ou une loi</li>
        <li>L'utiliser en tant qu'effet temporaire dans une page</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;del&gt;...&lt;/del&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="strikethrough"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-strikethrough fa-stack-1x fa-inverse"></span></span> Texte barré</h4>
  <p>L'utiliser pour indiquer du texte qui n'est plus pertinent.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Texte ordinaire et <s>texte barré</s>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li>L'utiliser pour montrer qu'une chose <strong>n'est plus exacte </strong>ou<strong> n'est plus pertinente</strong></li>
        <li>L'utiliser avec modération, puisqu'l rend une page difficile à lire</li>
        <li>L'utiliser pour montrer les modifications enregistrées dans un document officiel, comme un procès-verbal ou une loi</li>
        <li>L'utiliser en tant qu'effet temporaire dans une page</li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;s&gt;...&lt;/s&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="inserted"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-plus fa-stack-1x fa-inverse"></span></span> Texte inséré</h4>
  <p>L'utiliser pour indiquer des ajouts à un document. </p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Texte ordinaire et <ins>texte inséré</ins>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li><strong>N'utilisez pas cette fonction</strong>
          <ul>
            <li>Elle imite l'apparence visuelle d'un lien, ce qui cause des problèmes de convivialité</li>
            <li>Les éléments qui ne sont pas des liens <strong>ne doivent pas </strong>avoir l'apparence de liens</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;ins&gt;...&lt;/ins&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <h4 id="underlined"><span class="fa-stack"><span class="fa fa-circle fa-stack-2x"></span><span class="fa fa-underline fa-stack-1x fa-inverse"></span></span> Texte souligné</h4>
  <p>L'utiliser pour souligner du texte. N'utilisez pas cette fonction dans les pages Web.</p>
  <div class="row">
    <div class="col-md-4">
      <div class="panel panel-default">
        <div class="panel-body">
          <h5 class="mrgn-tp-0">Apparence</h5>
          <p>Texte ordinaire et  <u>texte souligné</u>.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0 text-success"><span class="glyphicon glyphicon-ok-circle"></span> Bonne utilisation</h5>
      <p><span class="nowrap">Points de conformité&nbsp;:</span></p>
      <ul>
        <li><strong>N'utilisez pas cette fonction</strong>
          <ul>
            <li>Elle imite l'apparence visuelle d'un lien, ce qui cause des problèmes de convivialité</li>
            <li>Les éléments qui ne sont pas des liens <strong>ne doivent pas </strong>avoir l'apparence de liens</li>
          </ul>
        </li>
      </ul>
      <h5 class="mrgn-tp-0 text-danger"><span class="glyphicon glyphicon-remove-circle"></span> Mauvaise utilisation</h5>
      <p><span class="nowrap">Point d'observation&nbsp;:</span></p>
      <ul>
        <li>N'utilisez pas cet élément d'une façon qui entre en conflit avec <span class="nowrap">les points</span>  d'observation  <span class="nowrap">précédents</span></li>
      </ul>
    </div>
    <div class="col-md-4">
      <h5 class="mrgn-tp-0">Code</h5>
      <pre><code>&lt;p&gt;...<strong>&lt;u&gt;...&lt;/u&gt;</strong>...&lt;/p&gt;</code></pre>
    </div>
  </div>
  <p class="mrgn-tp-lg text-muted">Une partie du code et des documents pour cette page est tirée de <a href="https://getbootstrap.com/" >Bootstrap<span  class="wb-inv"> (lien externe)</span></a>.</p>
{% endraw %}
{:/}
