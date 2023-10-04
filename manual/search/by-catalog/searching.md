# **RegulonDB Search**

[Gene](#by-gene)  
[Gensor Unit](#by-gu)  
[Growth Condition](#by-gc)  
[Operon](#by-operon)  
[Regulon](#by-regulon)  
[Sigmulon](#by-sigmulon)  


## Introduction

The five main Web pages (gene, operon, regulon, sigmulon, and GENSOR units) were redesigned to follow the same structure for a smoother browsing experience. As shown in Figure 8, they provide two options for searching, one using the box on the top right (see component 1 in the figure) when the user knows what object they are looking for, and the other on the left (see component 2 in the figure) that lists all objects to choose from. 


<center><img src="./images/searching_options.png
" alt="drawing" width="700"/></center>
Figure 8 illustrates the main web components utilized in creating the five key web pages mentioned: 1) The query box. 2) The catalog of elements where users can browse and search for specific items. 3) The object identification properties component. 4) The graphical representation component of the queried object. 5) The navigation menu for moving between sections of the page. 6) The related tools component. 7) The object details component.



### Searching box

One of the search options is through a search box, which allows you to search for a term (one or more words) in various fields where it can be found. This option is commonly used for identifiers, entity names, synonyms, among others. It also allows the use of logical operators.

| Logic operators | Description |
|:-- |:-- |
| OR  | Cuando se quieren hacer múltiples búsquedas en una consulta se utiliza el espacio (‘ ’) entre las palabras a buscar.|
| AND  | Cuando se quieren hacer búsquedas con múltiples palabras y se espera que estén en el mismo documento debe colocarse comillas escapeadas (‘/”’) a cada palabra. |
| NOT | Las búsquedas que quieren exceptuar palabras se les coloca un guion medio (‘-’) antes de la palabra a evadir. |





### <a name="by-gene">Gene</a>

You can use gene name, synonyms, identifiers, gene product, and GOs with the gene keyword. To get the complete list of the genes use only the keyword. 

araC _gene_

arabinose AND transporter AND _gene_

transcriptional regulator _gene_

b0012 _gene_

_gene_


### <a name="by-gu">Gensor Unit</a>

You can use the gensor unit name, the gensor unit identifier or the reaction name, with the gensor unit or gu keyword. To get the complete list of gensor units use only the keyword. 

araC _gensor unit_

PurR-hypoxanthine _gu_

_gensor unit_


### <a name="by-gc">Growth Condition</a>

You can use the condition identifier, the control, experimental and global condition with the growth condition keyword. To get the complete list of conditions use only the keyword. 

heat shock _growth condition_

glucose _growth condition_

_growth condition_


### <a name="by-operon">Operon</a>

You can use operon identifier, operon name, synonyms, transcription unit name, promoter name, promoter sequence with the operon keyword. To get the complete list of operons use only the keyword. 

lactose _operon_

metJ _operon_

glnALG _transcription unit_

_operon_


### <a name="by-regulon">Regulon</a>

You can use regulon identifier, regulon name, synonyms, transcription factor name, effector name, conformation of TFs with the operon keyword. To get the complete list of regulons use only the keyword, and you will get a table with the regulons and useful statistics. 

CRP _regulon_

Arabinose _regulon_

TyrR-tyrosine _regulon_

transcription AND factor AND repressor _regulon_

_regulon_


### <a name="by-sigmulon">Sigmulon</a>

You can use sigma name, sigma gene name and synonyms, with the sigmulon keyword. To get the complete list of sigmas use only the keyword. 

sigma19 _sigmulon_

rpoD _sigmulon_

_sigmulon_




