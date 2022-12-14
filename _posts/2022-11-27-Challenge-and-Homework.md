---
keywords: fastai
description: The homework assignment and challenge in our lesson plan
title: Challenge and Homework
toc: true 
comments: true
categories: [jupyter, Week 13]
nb_path: _notebooks/2022-11-27-Challenge-and-Homework.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-11-27-Challenge-and-Homework.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Challenge">Challenge<a class="anchor-link" href="#Challenge"> </a></h2><p>The list given contains multiple numbers with different values. There are also 2 variables that define the minimum and maximum valid values. Given these variables, output the values that do not fit into the valid range as well as their index values.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">data</span> <span class="o">=</span> <span class="p">[</span><span class="mi">104</span><span class="p">,</span> <span class="mi">101</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">105</span><span class="p">,</span> <span class="mi">308</span><span class="p">,</span> <span class="mi">103</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">107</span><span class="p">,</span>
        <span class="mi">100</span><span class="p">,</span> <span class="mi">306</span><span class="p">,</span> <span class="mi">106</span><span class="p">,</span> <span class="mi">102</span><span class="p">,</span> <span class="mi">108</span><span class="p">]</span>    <span class="c1"># list of the different numerical values</span>
<span class="n">min_valid</span> <span class="o">=</span> <span class="mi">100</span>  <span class="c1"># minimum value</span>
<span class="n">max_valid</span> <span class="o">=</span> <span class="mi">200</span>  <span class="c1"># maximum value</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)):</span>
        <span class="k">if</span> <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">&lt;</span><span class="n">min_valid</span> <span class="ow">or</span> <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">&gt;</span><span class="n">max_valid</span><span class="p">:</span>
                <span class="nb">print</span><span class="p">(</span><span class="n">i</span><span class="p">,</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>2 4
4 308
6 5
9 306
</pre>
</div>
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
<div class=" highlight hl-ipython3"><pre><span></span><span class="mi">9</span> <span class="mi">306</span>
<span class="mi">6</span> <span class="mi">5</span>
<span class="mi">4</span> <span class="mi">308</span>
<span class="mi">2</span> <span class="mi">4</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Homework/Hacks">Homework/Hacks<a class="anchor-link" href="#Homework/Hacks"> </a></h2><p>The list given contains 4 album names - Welcome to my Nightmare, Bad Company, Nightflight, More Mayhem - and each album contains at least 4 songs within another list. Given this, write a block of code that enables users to input in integer values that correspond to the albums and songs - Welcome to my Nightmare is 1, Bad Company is 2, etc. - Then, a sentence is outputted that says Playing <strong>___</strong> based on which song was chosen using the numbers inputted by the user that corresponds to each song.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">albums</span> <span class="o">=</span> <span class="p">[</span>
    <span class="p">(</span><span class="s2">&quot;Welcome to my Nightmare&quot;</span><span class="p">,</span> <span class="s2">&quot;Alice Cooper&quot;</span><span class="p">,</span> <span class="mi">1975</span><span class="p">,</span>   <span class="c1"># First album list</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;Welcome to my Nightmare&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Devil&#39;s Food&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;The Black Widow&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;Some Folks&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="s2">&quot;Only Women Bleed&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
    <span class="p">(</span><span class="s2">&quot;Bad Company&quot;</span><span class="p">,</span> <span class="s2">&quot;Bad Company&quot;</span><span class="p">,</span> <span class="mi">1974</span><span class="p">,</span>   <span class="c1"># Second album list</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;Can&#39;t Get Enough&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Rock Steady&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;Ready for Love&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;Don&#39;t Let Me Down&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="s2">&quot;Bad Company&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">6</span><span class="p">,</span> <span class="s2">&quot;The Way I Choose&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">7</span><span class="p">,</span> <span class="s2">&quot;Movin&#39; On&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="s2">&quot;Seagull&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
    <span class="p">(</span><span class="s2">&quot;Nightflight&quot;</span><span class="p">,</span> <span class="s2">&quot;Budgie&quot;</span><span class="p">,</span> <span class="mi">1981</span><span class="p">,</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;I Turned to Stone&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Keeping a Rendezvous&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;Reaper of the Glory&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;She Used Me Up&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
    <span class="p">(</span><span class="s2">&quot;More Mayhem&quot;</span><span class="p">,</span> <span class="s2">&quot;Imelda May&quot;</span><span class="p">,</span> <span class="mi">2011</span><span class="p">,</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;Pulling the Rug&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Psycho&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;Mayhem&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;Kentish Town Waltz&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
<span class="p">]</span>
<span class="n">album</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">())</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choosing album&quot;</span><span class="p">,</span> <span class="n">album</span><span class="p">)</span>
<span class="n">song</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">())</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choosing song&quot;</span><span class="p">,</span> <span class="n">song</span><span class="p">)</span>
<span class="k">try</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Playing&quot;</span><span class="p">,</span><span class="n">albums</span><span class="p">[</span><span class="n">album</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">3</span><span class="p">][</span><span class="n">song</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">])</span>
<span class="k">except</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;That song is not in the playlist&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Choosing album 2
Choosing song 2
Playing Rock Steady
</pre>
</div>
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
<div class=" highlight hl-ipython3"><pre><span></span><span class="mi">1</span>
<span class="mi">1</span>
<span class="n">Playing</span> <span class="s2">&quot;Welcome to my Nightmare&quot;</span>

<span class="mi">2</span>
<span class="mi">2</span>
<span class="n">Playing</span> <span class="s2">&quot;Rock Steady&quot;</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

</div>
 

