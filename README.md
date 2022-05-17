# WiRe57

This repository contains resources for the Open Information Extraction benchmark **WiRe57**.

It acts as a companion to the article

William Léchelle, Fabrizio Gotti, Philippe Langlais (2019), [*WiRe57 : A Fine-Grained Benchmark for Open Information Extraction*](https://arxiv.org/abs/1809.08962), LAW XIII 2019 : The 13th Linguistic Annotation Workshop
 
# Introduction
Open  Information  Extraction  (OIE) systems,  starting with [TextRunner](http://www.aclweb.org/anthology/N07-4013), seek to extract all relational tuples expressed in text, without being  bound to an  anticipated  list  of  predicates. Such  systems  have  been  used  recently  for relation extraction, question-answering,  and  for  building domain-targeted knowledge bases, among others.

Subsequent  extractors  ([ReVerb](http://www.aclweb.org/anthology/D11-1142), [Ollie](https://www.aclweb.org/anthology/D12-1048), [ClausIE](https://dl.acm.org/citation.cfm?id=2488420), [Stanford Open IE](https://nlp.stanford.edu/pubs/2015angeli-openie.pdf), [OpenIE4](https://www.ijcai.org/Proceedings/16/Papers/604.pdf), [MinIE](http://aclweb.org/anthology/D17-1278)) have sought to improve  yield and  precision. Despite this, the task definition is underspecified,  and,  to  the  best  of  our knowledge,  there is no gold standard.

In order to mitigate this problem, we built a reference for the task of Open Information Extraction, on five documents. We tentatively resolve a number of issues that arise, including inference and granularity. We seek to better pinpoint the requirements for the task. We produce our annotation guidelines specifying what is correct to extract and what is not. In turn, we use this reference to score existing Open IE systems. We address the non-trivial problem of evaluating the extractions produced by systems against the reference tuples, and share our evaluation script. Among seven compared extractors, we find the MinIE system to perform best.

# Available resources

The [annotation guidelines](https://docs.google.com/document/d/1DI4r8NpeS0-ZtHP24Q_oioQh0xyYK6vIjKrKmeNo-aE/edit) define how to annotate English text with triples.

The `data` directory contains the following files:
* `README.md`: Specifies the source of the annotated documents.
* `WiRe57_343-manual-oie.json`: The WiRe57 manual reference
* `WiRe57_extractions_by_ollie_clausie_openie_stanford_minie_reverb_props-export.json`: Extractions by state-of-the-art OIE systems on WiRe documents.

The `code` directory contains the evaluation script used in the paper. 
