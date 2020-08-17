---
keywords: fastai
description: Initiation aux listes en python
title: Découverte des objets listes
toc: true
badges: true
comments: false
categories: [python, ISN]
nb_path: _notebooks/2020-03-07-Python2 - Introduction aux listes.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2020-03-07-Python2 - Introduction aux listes.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Les listes sont des objets très importants en Python car elles permettent de stocker de multiples informations dans une seule variable.</p>
<p>Ci dessous, voici un exemple montrant la liste des entiers de 0 à 9.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">list</span><span class="p">(</span><span class="nb">range</span><span class="p">(</span><span class="mi">10</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Nous allons dans ce chapitre détailler ce qu'est une liste, comment les manipuler et expliquer pourquoi elles sont si importantes en Informatique.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Manipulation-de-listes">Manipulation de listes<a class="anchor-link" href="#Manipulation-de-listes"> </a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Pr&#233;sentation-du-type-list">Pr&#233;sentation du type list<a class="anchor-link" href="#Pr&#233;sentation-du-type-list"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Comme on peut le voir sur l'exemple précédent, une <strong>liste</strong> en Python est un objet délimité par deux crochets et qui renferme un nombre fini d'éléments de n'importe quel type, ces éléments étant séparés par des virgules.</p>
<p>Voici quelques caractéristiques sur les listes</p>
<blockquote><ul>
<li>les éléments d'une liste sont ordonnés :si on échange de place deux éléments différents d'une liste, la liste est modifiée.&gt;- les éléments d'une liste sont numérotés <strong>depuis 0</strong></li>
<li>un même objet peut appparaître plusieurs fois dans une liste.</li>
<li>une liste peut contenir des éléments de type différents (nombres, chaines...)</li>
</ul>
</blockquote>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">Premier_Exemple</span><span class="o">=</span><span class="p">[</span><span class="mi">21</span><span class="p">,</span><span class="s2">&quot;Bonjour&quot;</span><span class="p">,</span><span class="mi">1</span><span class="o">+</span><span class="mi">2</span><span class="p">,[</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">1</span><span class="p">],</span> <span class="mi">21</span> <span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="n">Premier_Exemple</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">Premier_Exemple</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Premi&#232;res-manipulations-sur-les-listes">Premi&#232;res manipulations sur les listes<a class="anchor-link" href="#Premi&#232;res-manipulations-sur-les-listes"> </a></h3><p>Créez une variable <strong><em>liste_carres</em></strong> contenant la liste les carrés des entiers de 1 à 10</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">liste_carres</span> <span class="o">=</span> <span class="o">...</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">assert</span> <span class="mi">81</span> <span class="ow">in</span> <span class="n">liste_carres</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Les éléments d'une liste sont numérotés à partir de 0. On accède à un élément en utilisant une notation crochet : <strong><em>maListe[index]</em></strong>.</p>
<p>Observez l'exemple et modifiez le pour accéder aux différents éléments de la <strong><em>liste_carres</em></strong></p>
<p>Observez le message d'erreur lorsque l'index dépasse le nombre d'éléments dans la liste !</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">liste_carres</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">liste_carres</span><span class="p">[</span><span class="mi">11</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Il est possible de modifier un élément particulier d'une liste. Il suffit de faire une affectation au moyen du signe = comme pour une simple variable. Observez plutôt :</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">liste_carres</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">=</span><span class="mi">100</span>
<span class="nb">print</span><span class="p">(</span><span class="n">liste_carres</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut rechercher si un élément dans une liste. Par exemple pour savoir si 25 est un carré, on peut taper la ligne suivante.</p>
<p>Manipulez cette fonction en testant des nombres qui sont dans la liste et d'autres qui n'y sont pas.</p>
<p>On sera frappé par la similitude entre la syntaxe de python et le langage naturel. Cette simplicité est une des forces de Python.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="mi">25</span> <span class="ow">in</span> <span class="n">liste_carres</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut mettre deux listes bout à bout comme on le voit sur l'exemple suivant. On remarque l'utilisation naturelle du signe '+' pour ajouter deux listes bout à bout.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">liste_carres</span><span class="o">=</span><span class="n">liste_carres</span> <span class="o">+</span> <span class="p">[</span><span class="mi">121</span><span class="p">,</span><span class="mi">144</span><span class="p">,</span><span class="mi">169</span><span class="p">,</span><span class="mi">196</span><span class="p">,</span><span class="mi">225</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="n">liste_carres</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>De même qu'on possède l'opération +, il existe aussi l'opération * pour obtenir une liste formée de plusieurs fois la même liste. Je vous laisse découvrir le fonctionnement de cet opérateur dans la cellule ci-dessous :</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="mi">3</span><span class="o">*</span><span class="p">[</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">4</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour savoir combien d'éléments contient une liste, on peut utiliser la fonction <strong><em>len()</em></strong>.</p>
<p>Testez aussi les fonctions <strong><em>min()</em></strong> et <strong><em>max()</em></strong> sur la liste_carres. A quoi servent elles ?</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">len</span><span class="p">(</span><span class="n">liste_carres</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="nb">min</span><span class="p">(</span><span class="n">liste_carres</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="nb">max</span><span class="p">(</span><span class="n">liste_carres</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour connaître la position d'un objet dans une liste, on peut utiliser la méthode <strong>*.index()</strong>. Elle s'utilise comme suit. Que se passe t-il si l'objet recherché n'appartient pas à la liste ?</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">liste_carres</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="mi">81</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>De la même manière, on peut compter le nombre d'éléments dans une liste. Pour cela, on utilise la méthode <strong><em>.count()</em></strong> de manière similaire à <strong><em>.index()</em></strong>. Pour vous exercer, ajouter à <strong><em>liste_carres</em></strong> la liste [121,81,169,81] et comptez le nombre d'occurences du nombre 81.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># A vous de jouer dans cette cellule</span>
<span class="n">liste_carres</span><span class="o">=...</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Parcourir-une-liste">Parcourir une liste<a class="anchor-link" href="#Parcourir-une-liste"> </a></h3><p>Il existe deux manières de parcourir une liste :</p>
<ul>
<li>le parcours élément par élément</li>
<li>le parcours par index</li>
</ul>
<p>Dans les deux cas on utilisera une boucle <em>pour</em>. Observez les exemples suivants :</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Parcours élément par élément</span>
<span class="k">for</span> <span class="n">elmt</span> <span class="ow">in</span> <span class="n">liste_carres</span><span class="p">:</span>
    <span class="nb">print</span> <span class="p">(</span><span class="s2">&quot;ce nombre est un carré : &quot;</span><span class="p">,</span><span class="n">elmt</span><span class="p">)</span>
    
<span class="c1"># Parcours par index</span>
<span class="n">longueur_liste</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">liste_carres</span><span class="p">)</span>
<span class="k">for</span> <span class="n">indx</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">longueur_liste</span><span class="p">):</span>
    <span class="nb">print</span> <span class="p">(</span><span class="s2">&quot;ce nombre est aussi un carré : &quot;</span><span class="p">,</span><span class="n">liste_carres</span><span class="p">[</span><span class="n">indx</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Dans le parcours par élément, la variable de boucle <strong>contient les différents éléments</strong> de la liste. Dans le second parcours par index, la variable de boucle est l'<strong>index permettant d'accéder à l'élément</strong>. Il faut dans ce cas commencer par déterminer la longueur de la liste pour ne pas risquer un dépassement d'index.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Exercice-1">Exercice 1<a class="anchor-link" href="#Exercice-1"> </a></h3><ol>
<li><p>Ecrire une fonction <strong>etendue</strong></p>
<ul>
<li>prenant en paramètre une liste de nombres</li>
<li>renvoyant l'étendue de cette liste à savoir l'écart entre la plus grande valeur et la plus petite valeur</li>
</ul>
</li>
<li><p>Ecrire une fonction <strong>somme</strong></p>
<ul>
<li>prenant en argument une liste </li>
<li>renvoyant la somme de tous les termes de la liste</li>
</ul>
</li>
<li><p>Ecrire une fonction <strong>moyenne</strong></p>
<ul>
<li>prenant en paramètre une liste de nombres</li>
<li>renvoyant la valeur moyenne des nombres de la liste</li>
</ul>
</li>
</ol>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># YOUR CODE HERE</span>
<span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La cellule de tests suivante doit s'exécuter sans erreur</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">assert</span> <span class="n">somme</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="mi">30</span><span class="p">)))</span> <span class="o">==</span> <span class="mi">435</span>
<span class="k">assert</span> <span class="n">etendue</span><span class="p">([</span><span class="mi">3</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">9</span><span class="p">,</span><span class="mi">4</span><span class="p">,</span><span class="mi">5</span><span class="p">])</span><span class="o">==</span><span class="mi">8</span>
<span class="k">assert</span> <span class="n">moyenne</span><span class="p">([</span><span class="mi">3</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">9</span><span class="p">,</span><span class="mi">4</span><span class="p">,</span><span class="mi">5</span><span class="p">])</span><span class="o">==</span><span class="mf">4.4</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Modification-d'une-liste">Modification d'une liste<a class="anchor-link" href="#Modification-d'une-liste"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour modifier une liste, il suffit d'effectuer une affectation à l'un de ses éléments via son index. Observez les exemples ci-dessous. Que signifie l'index -1 dans une liste ?</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">L</span><span class="o">=</span><span class="p">[[</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">],</span><span class="s2">&quot;bonjour&quot;</span><span class="p">,</span><span class="mi">3</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Liste initiale &quot;</span><span class="p">,</span><span class="n">L</span><span class="p">)</span>
<span class="n">L</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">=</span><span class="p">[</span><span class="mi">6</span><span class="p">,</span><span class="mi">8</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Premier élément modifié :&quot;</span><span class="p">,</span><span class="n">L</span><span class="p">)</span>
<span class="n">L</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">=</span><span class="s2">&quot;au revoir&quot;</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Qu&#39;est-ce qui a changé ?&quot;</span><span class="p">,</span> <span class="n">L</span><span class="p">)</span>
<span class="n">L</span><span class="p">[</span><span class="mi">0</span><span class="p">][</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">=</span><span class="mi">9</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;On modifie le premier élément :&quot;</span><span class="p">,</span><span class="n">L</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Les-m&#233;thodes-sur-les-listes">Les m&#233;thodes sur les listes<a class="anchor-link" href="#Les-m&#233;thodes-sur-les-listes"> </a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Il existe encore d'autres moyens de manipulation de listes.</p>
<p>Il existe en fait des fonctions intégrées à la structure de listes permettant d'agir sur celles-ci : on les nomme <strong>méthodes</strong> et leur syntaxe générale est, étant donnée une liste $L$ :</p>
<p>$L.Methode()$, où $Methode()$ fait référence à l'une des méthodes détaillée ci-dessous.</p>
<p>Il est à noter qu'une fois la ligne $L.Methode()$ executée, la liste $L$ est, en général, transformée en sa liste modifiée.</p>
<p>Ces méthodes revoient à la programmation orientée objet de Python : les listes sont des objets qui sont manipulés, modifiés selon certains transformations et évoluent au grés de ces modifications.</p>
<p>Voici un petit catalogue des méthodes utiles. Vous retrouverez des méthodes déjà vues ci-dessus.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="La-m&#233;thode-.append()">La m&#233;thode .append()<a class="anchor-link" href="#La-m&#233;thode-.append()"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La syntaxe  $L.append(objet)$ ajoute $objet$ à droite dans $L$ :</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">L</span><span class="o">=</span><span class="p">[</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">4</span><span class="p">]</span>
<span class="n">L</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="mi">5</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>  <span class="c1"># la liste initiale vient d&#39;être modifiée !</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="La-m&#233;thode-.insert()">La m&#233;thode .insert()<a class="anchor-link" href="#La-m&#233;thode-.insert()"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La syntaxe $L.insert(Indice,objet)$ insère $objet$ en place $Indice$ dans la liste $L$ et décale le reste des occurrences de $L$ à droite :</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">L</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;Pomme&quot;</span><span class="p">,</span><span class="s2">&quot;Poire&quot;</span><span class="p">,</span><span class="s2">&quot;Banane&quot;</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>
<span class="n">L</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="s2">&quot;Fraise&quot;</span><span class="p">)</span> <span class="c1"># vient prendre la place de &quot;Poire&quot;</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>
<span class="n">L</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span><span class="s2">&quot;Ananas&quot;</span><span class="p">)</span> <span class="c1"># vient prendre la place de &quot;Banane&quot;</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="La-m&#233;thode-.remove()">La m&#233;thode .remove()<a class="anchor-link" href="#La-m&#233;thode-.remove()"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La syntaxe  $L.remove(objet)$ supprime de la liste la première occurrence égale à $objet$ dans la liste $L$. Si $objet$ n'est pas présent dans $L$, cela produit un message d'erreur.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">M</span><span class="o">=</span><span class="p">[</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="n">M</span><span class="p">)</span>
<span class="n">M</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="mi">2</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">M</span><span class="p">)</span>  <span class="c1"># seul le premier &quot;2&quot; est supprimé !</span>
<span class="n">M</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="mi">3</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">M</span><span class="p">)</span>  <span class="c1"># seul le premier &quot;3&quot; est supprimé !</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="La-m&#233;thode-.pop()">La m&#233;thode .pop()<a class="anchor-link" href="#La-m&#233;thode-.pop()"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La syntaxe  $L.pop([Indice])$ renvoie $L[Indice]$ et supprime l'élément d'index $Indice$ de la liste $L$. Il n'est pas nécessaire que  $Indice$ soit dans les bornes cycliques licites entre $-len(L)$ et $len(L)-1$, mais cela est quand même conseillé pour une meilleure lecture du script.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">L</span><span class="o">=</span><span class="p">[</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="s2">&quot;mot&quot;</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">6</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>
<span class="n">L</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>
<span class="n">L</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">3</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">L</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="La-m&#233;thode-.index()">La m&#233;thode .index()<a class="anchor-link" href="#La-m&#233;thode-.index()"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La syntaxe $L.index(objet)$ renvoie l'index de la première occurrence d'$objet$ dans $L$. La liste $L$ n'est pas modifiée par cette méthode. Cela renvoie un message d'erreur lorsque $objet$ ne figure pas dans la liste $L$.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">Liste</span><span class="o">=</span><span class="p">[</span><span class="mi">2</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="s2">&quot;un mot&quot;</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">2</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="n">Liste</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">Liste</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;un mot&quot;</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="n">Liste</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="mi">3</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="n">Liste</span><span class="p">)</span>  <span class="c1"># liste non modifiée</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="La-m&#233;thode-.count()">La m&#233;thode .count()<a class="anchor-link" href="#La-m&#233;thode-.count()"> </a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La syntaxe $L.count(objet)$ renvoie le nombre d'occurrences égales à $objet$ dans la liste $L$. Cele ne modifie pas la liste initiale.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">Liste</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="mi">2</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Tranches-de-listes">Tranches de listes<a class="anchor-link" href="#Tranches-de-listes"> </a></h3><p>Etant donnée une liste $L$, la syntaxe $L[Indice$<em>$Debut:Indice$</em>$Fin:Pas]$ renvoie la sous-liste composée des termes $L[k]$, où l'indice $k$ vaut successivement $Indice$<em>$Debut$,$Indice$</em>$Debut$+$Pas$, $Indice$<em>$Debut$+2 $Pas$, etc. On s'arrête avant d'avoir atteint $Indice$</em>$Fin$. Le dernier indice n''est jamais inclus dans la sélection.</p>
<p>Il est à noter que $Pas$ peut être strictement négatif. Regardez attentivement les exemples suivants. N'hésitez pas à les modifier pour observer l'influence de chaque indice.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">L</span><span class="o">=</span><span class="nb">list</span><span class="p">(</span><span class="nb">range</span><span class="p">(</span><span class="mi">30</span><span class="p">))</span> <span class="c1"># list() trasnforme un objet en liste</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;affichage de toute la liste : &quot;</span><span class="p">,</span><span class="n">L</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;une liste du troisième au dixième terme :&quot;</span><span class="p">,</span><span class="n">L</span><span class="p">[</span><span class="mi">2</span><span class="p">:</span><span class="mi">10</span><span class="p">])</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;affichage de certains termes : &quot;</span><span class="p">,</span> <span class="n">L</span><span class="p">[</span><span class="mi">3</span><span class="p">:</span><span class="mi">28</span><span class="p">:</span><span class="mi">6</span><span class="p">])</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;affichage sans le premier terme :&quot;</span><span class="p">,</span> <span class="n">L</span><span class="p">[</span><span class="mi">1</span><span class="p">:])</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;affichage des cinq premiers termes :&quot;</span><span class="p">,</span><span class="n">L</span><span class="p">[:</span><span class="mi">5</span><span class="p">])</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;la liste dans le sens inverse :&quot;</span><span class="p">,</span><span class="n">L</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Exercice-2-:-Simulation-de-lancer-de-d&#233;">Exercice 2 : Simulation de lancer de d&#233;<a class="anchor-link" href="#Exercice-2-:-Simulation-de-lancer-de-d&#233;"> </a></h3><ol>
<li>Ecrire une fonction <strong>genere_liste</strong> <ul>
<li>prenant en paramètre un entier $n$</li>
<li>renvoyant une liste de $n$ nombres aléatoires entre 1 et 6</li>
</ul>
</li>
<li>Ecrire une fonction <strong>frequence_6</strong><ul>
<li>prenant en paramètre une liste de nombres</li>
<li>renvoyant la fréquence d'apparition du 6</li>
</ul>
</li>
</ol>
<p><em>Indication</em> : On pourra utiliser les commandes suivantes pour tirer un nombre aléatoire entre 1 et 6 :</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">random</span> <span class="kn">import</span> <span class="o">*</span> <span class="c1"># A mettre au début du programme</span>

<span class="n">randint</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="mi">6</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">random</span> <span class="kn">import</span> <span class="o">*</span> <span class="c1"># A mettre au début du programme</span>

<span class="c1"># YOUR CODE HERE</span>
<span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

</div>
 
