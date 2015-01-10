--- 
name: phylogenetic-community-structure-pglmms
layout: post
title: "Phylogenetic community structure: PGLMMs"
author: Scott Chamberlain
date: 2011-10-13 10:18:00.001000 -05:00
tags: 
- Evolution
- Papers
- Ecology
- Statistics
- Picante
- R
---
So, <a href="http://r-ecology.blogspot.com/2011/01/new-approach-to-analysis-of.html">I've blogged about this topic before</a>, way back on 5 Jan this year.<br /><br />Matt Helmus, a postdoc in the <a href="http://woottonlab.uchicago.edu/">Wootton lab at the University of Chicago</a>, published a paper with Anthony Ives in Ecological Monographs this year (<a href="http://www.esajournals.org/doi/abs/10.1890/10-1264.1">abstract here</a>). &nbsp;The paper addressed a new statistical approach to phylogenetic community structure. <br /><br />As I said in the original post, part of the power of the PGLMM (phylogenetic generalized linear mixed models) approach is that you don't have to conduct quite so many separate statistical tests as with the previous null model/randomization approach. <br /><br />Their original code was written in Matlab. &nbsp;Here I provide the R code that Matt has so graciously shared with me. &nbsp;There are four functions and a fifth file has an example use case. &nbsp;The example and output are shown below. <br /><br />Look for the inclusion of Matt's PGLMM to the picante R package in the future.<br /><br /><u>Here are links to the files as GitHub gists:&nbsp;</u><br />PGLMM.data.R: &nbsp;<a href="https://gist.github.com/1278205">https://gist.github.com/1278205</a><br />PGLMM.fit.R: &nbsp;<a href="https://gist.github.com/1284284">https://gist.github.com/1284284</a><br />PGLMM.reml.R: &nbsp;<a href="https://gist.github.com/1284287">https://gist.github.com/1284287</a><br />PGLMM.sim.R: &nbsp;<a href="https://gist.github.com/1284288">https://gist.github.com/1284288</a><br />PGLMM_example.R: &nbsp;<a href="https://gist.github.com/1284442">https://gist.github.com/1284442</a><br /><br />Enjoy!<br /><br /><br /><b><u>The example</u></b><br /><script src="https://gist.github.com/1284477.js?file=PGLMM_exampleoutput.R"></script><br /><br /><br />..and the figures...<br /><div class="separator" style="clear: both; text-align: center;"><a href="http://3.bp.blogspot.com/-ODHXaozYSFY/Tpb9qSXbbHI/AAAAAAAAFDg/hLHlGDiYRSw/s1600/plot1.png" imageanchor="1" style="clear: left; float: left; margin-bottom: 1em; margin-right: 1em;"><img border="0" height="315" src="http://3.bp.blogspot.com/-ODHXaozYSFY/Tpb9qSXbbHI/AAAAAAAAFDg/hLHlGDiYRSw/s320/plot1.png" width="320" /></a></div><br /><div class="separator" style="clear: both; text-align: center;"><a href="http://2.bp.blogspot.com/-tQYXCZWIMYs/Tpb9q5zF4EI/AAAAAAAAFDo/_iOxMYf5DsI/s1600/plot2.png" imageanchor="1" style="clear: left; float: left; margin-bottom: 1em; margin-right: 1em;"><img border="0" height="307" src="http://2.bp.blogspot.com/-tQYXCZWIMYs/Tpb9q5zF4EI/AAAAAAAAFDo/_iOxMYf5DsI/s320/plot2.png" width="320" /></a></div><br /><div class="separator" style="clear: both; text-align: center;"><a href="http://1.bp.blogspot.com/-fowoTDI0chc/Tpb9rMAlswI/AAAAAAAAFDw/7pvqZ-jpECk/s1600/plot3.png" imageanchor="1" style="clear: left; float: left; margin-bottom: 1em; margin-right: 1em;"><img border="0" height="320" src="http://1.bp.blogspot.com/-fowoTDI0chc/Tpb9rMAlswI/AAAAAAAAFDw/7pvqZ-jpECk/s320/plot3.png" width="316" /></a></div><br />