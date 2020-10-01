---
title: ""
--author: "RegulonDB Team"
--date: '02/07/2020'
output:
  html_document:
    fig_caption: yes
    highlight: zenburn
    includes:
    css: ../../css/regulondbGlobalStyle.css
    self_contained: yes
---

<div style="text-align: center"> 
<h1>RegulonDB Searching Help</h1>
</div>



### Searching by Coexpression

A list of genes (gene name), separated by space or commas, can be introduced.            

&nbsp;&nbsp;&nbsp;&nbsp; araA araB araD AraC *coexpression*  
&nbsp;&nbsp;&nbsp;&nbsp; soda, soxS, soxR *coexpression*                



### RegulonDB uses ElasticSearch as a full-text search engine.



### Searching by Gene {#searching-by-gen}
You can use gene name, synonyms, identifiers, gene product, and GOs with the gene keyword. To get the complete list of the genes use only the keyword.            

&nbsp;&nbsp;&nbsp;&nbsp; araC *gene*  
&nbsp;&nbsp;&nbsp;&nbsp; arabinose AND transporter AND *gene*  
&nbsp;&nbsp;&nbsp;&nbsp; transcriptional regulator *gene*  
&nbsp;&nbsp;&nbsp;&nbsp; b0012 *gene*  
&nbsp;&nbsp;&nbsp;&nbsp; *gene*                




### Searching by Gensor Unit {#searching-by-gu}
You can use the gensor unit name, the gensor unit identifier or the reaction name, with the gensor unit or gu keyword. To get the complete list of gensor units use only the keyword.            

&nbsp;&nbsp;&nbsp;&nbsp; araC *gensor unit*  
&nbsp;&nbsp;&nbsp;&nbsp; PurR-hypoxanthine *gu*  
&nbsp;&nbsp;&nbsp;&nbsp; *gensor unit*               





### Searching by Growth Condition {#searching-by-gc}
You can use the condition identifier, the control, experimental and global condition with the growth condition keyword. To get the complete list of conditions use only the keyword.            

&nbsp;&nbsp;&nbsp;&nbsp; heat shock *growth condition*  
&nbsp;&nbsp;&nbsp;&nbsp; glucose *growth condition*  
&nbsp;&nbsp;&nbsp;&nbsp; *growth condition*                





### Searching by Operon {#searching-by-operon}
You can use operon identifier, operon name, synonyms, transcription unit name, promoter name, promoter sequence with the operon keyword. To get the complete list of operons use only the keyword.            

&nbsp;&nbsp;&nbsp;&nbsp; lactose *operon*  
&nbsp;&nbsp;&nbsp;&nbsp; metJ *operon*  
&nbsp;&nbsp;&nbsp;&nbsp; glnALG *transcription unit*  
&nbsp;&nbsp;&nbsp;&nbsp;  *operon*                





### Searching by Regulon {#searching-by-regulon}
You can use regulon identifier, regulon name, synonyms, transcription factor name, effector name, conformation of TFs with the operon keyword. To get the complete list of regulons use only the keyword, and you will get a table with the regulons and useful statistics.            

&nbsp;&nbsp;&nbsp;&nbsp; CRP *regulon*  
&nbsp;&nbsp;&nbsp;&nbsp; Arabinose *regulon*  
&nbsp;&nbsp;&nbsp;&nbsp; TyrR-tyrosine *regulon*  
&nbsp;&nbsp;&nbsp;&nbsp; transcription AND factor AND repressor *regulon*  
&nbsp;&nbsp;&nbsp;&nbsp; *regulon*                





### Searching by Sigmulon {#searching-by-sigmulon}
You can use sigma name, sigma gene name and synonyms, with the sigmulon keyword. To get the complete list of sigmas use only the keyword.            

&nbsp;&nbsp;&nbsp;&nbsp; sigma19 *sigmulon*  
&nbsp;&nbsp;&nbsp;&nbsp; rpoD *sigmulon*  
&nbsp;&nbsp;&nbsp;&nbsp; *sigmulon*                





### Searching by sRNA {#searching-by-srna}
You can use sRNA name, product name and synonyms, with the sRNA or small RNA keywords. To get the complete list of sRNA use only the keyword.            

&nbsp;&nbsp;&nbsp;&nbsp; micF *sRNA*  
&nbsp;&nbsp;&nbsp;&nbsp; omrB *small RNA*  
&nbsp;&nbsp;&nbsp;&nbsp; *sRNA*                