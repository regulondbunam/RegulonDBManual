# **RegulonDB Search**

[Gene](#by-gene)  
[Gensor Unit](#by-gu)  
[Growth Condition](#by-gc)  
[Operon](#by-operon)  
[Regulon](#by-regulon)  
[Sigmulon](#by-sigmulon)  


## Introduction

The five main Web pages (gene, operon, regulon, sigmulon, and GENSOR units) were redesigned to follow the same structure for a smoother browsing experience. As shown in Figure below, they provide two options for searching, one using the box on the top right (see component 1 in the figure) when the user knows what object they are looking for, and the other on the left (see component 2 in the figure) that lists all objects to choose from. 


<center><img src="./images/searching_options.png
" alt="drawing" width="700"/></center>
Figure. illustrates the main web components utilized in creating the five key web pages mentioned: 1) The query box. 2) The catalog of elements where users can browse and search for specific items. 3) The object identification properties component. 4) The graphical representation component of the queried object. 5) The navigation menu for moving between sections of the page. 6) The related tools component. 7) The object details component.



### Searching box

One of the search options is through a searching box (see 1 in the figure), which allows you to search for a term (one or more words) in various fields where it can be found. This option is commonly used for identifiers, entity names, synonyms, among others. It also allows the use of logical operators.

| Logic operators | Description |
|:-- |:-- |
| OR  | The OR operator tells the search engine to return documents if they contain one or more keywords. In the query box you can use  OR operator or ' ' space. For example `araC OR araJ`  or  `AraC araJ` |
| AND  | The AND operator tells the search engine to return only documents with all the keywords you entered. For example `transcriptional AND activator`|
| NOT |The NOT operator (or "-") tells the search engine to exclude documents from a search if they contain the keywords. For example `transcriptional NOT activator` |


<br>

### Searching by Catalog

Another way to perform searches is by using the catalogs (see 2 in the figure). You can find them on the main page as links below the search box, or from the Search menu under `Search by Catalog`. When selecting an object (Gene, Operon, Regulon, etc.), the complete list of available records in the data collections will be displayed. The data will be shown by pagination, with additional information that may be helpful in selecting the record you are looking for. 

<br>
<br>

## <a name="by-gene">Gene</a>

The examples below apply to searching from the search box. You can use the gene name, synonyms, identifiers, gene product, and GOs as search terms.

Examples

> Using gene name: `araC gene`
> 
> Using produt name: transcriptional regulator _gene_
> 
> Using locus tag: `b0012 gene`

> arabinose AND transporter AND _gene_



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




