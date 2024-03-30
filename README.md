# aXa-trees
aXa stands for _arbustum_ ΧΡΙΣΤΙΑΝΩΝ _antiquorum_, "ancient forest of Christians". Its symbol is a _nomen sacrum_ evoking ancient scribal practices and a nod to the centrality of Christian scripture in historical corpus linguistics.

## The Problem
While many other treebanks of New Testament texts exist, they do not conform to established international standards, and thus make parsing and comparison with broader Greek linguistic corpora difficult.

## The Background 
These treebanks simultaneously follow and adopt both of the leading international standards for syntactical treebanks: Universal Dependencies (UD) and Ancient Greek and Latin Dependency (AGDT). The UD standard is itself a combination, specifically of the Stanford dependencies and Google universal tags, and now extends to test/train data and models in over 200 languages. The AGDT standard was developed among leading scholars of Classical Greek and Latin, and it boasts the greatest amount of gold-standard, expert-tagged syntactical data of Classical Greek in the world (over 500k tokens), with millions more tokens produced in a largely identical format by the GlauX project.

## The Purpose
By adopting both UD and AGDT formats, then aligning and combining them into a single representation, we maximize the potential for cross-validation, for the use of these treebanks as crosswalks between the two leading formats, and for broad accessibility and comparison within computational linguistic analyses and applications.

## The Credits
These postclassical Greek syntactical trees (aka dependency treebanks) are (to varying degrees) typically based on earlier openly licensed treebanks and projects as detailed below.

### PROIEL - Universal Dependencies format - CoNLL-U
The PROIEL treebanks include most Greek New Testament texts based on the Editio Octava (Eighth Edition) of the Greek New Testament (GNT) by Constantin Tischendorf (1869/1872), a work now in the public domain. The latest version of the PROIEL xml and conllu files may be found in the [Syntacticus repo](https://github.com/syntacticus/syntacticus-treebank-data/blob/main/proiel/greek-nt.conll). The conllu data used in this repo are largely derived from the tripartite-split files used in the [Universal Treebanks PROIEL model]( https://universaldependencies.org/treebanks/grc_proiel/index.html). When specific verses, chapter, or books are missing, these are added from text processed using the UDpipe PROIEL model, with expert edits and corrections as needed. The PROIEL Treebank is freely available under a [CC BY-NC-SA 3.0 license](http://creativecommons.org/licenses/by-nc-sa/3.0/us/).

> Dag T. T. Haug and Marius L. Jøhndal. 2008. 'Creating a Parallel Treebank of the Old Indo-European Bible Translations'. In Caroline Sporleder and Kiril Ribarov (eds.). Proceedings of the Second Workshop on Language Technology for Cultural Heritage Data (LaTeCH 2008) (2008), pp. 27-34. [doi:10.5281/zenodo.10655061](https://doi.org/10.5281/zenodo.10655061).

### GlauX - Ancient Greek and Latin Dependency format - XML
The GlauX treebanks of New Testament texts were produced based on the manual tagging of the PROIEL project, again following Tischendorf's GNT, with automated, semi-automated, and manual transformations applied. The Glaux treebanks follow the AGDT standard in most respects, and were produced under the expert direction of Toon van Haal and Alek Keersmaekers at KU-Leuven. They are (or soon will be) available in Glaux repos under a [CC0 1.0 license](https://github.com/perseids-publications/glaux-trees/blob/master/TREEBANK_LICENSE). For a representative publication of their work, see:

> Keersmaekers A, Van Hal T. Creating a large-scale diachronic corpus resource: Automated parsing in the Greek papyri (and beyond). Natural Language Engineering. Published online 2023:1-30. [doi:10.1017/S1351324923000384](https://doi.org/10.1017/S1351324923000384).

## The Invitation
Collaborators are welcome to join in our efforts to curate gold-standard UD- and AGDT-treebanks of early Christian texts. The most effective way to contribute is to make pull requests and propose edits to the edited source files (xml and conllu), rather than the original files or the combined output, since the original files are needed for reference and the combined output is generated with a scripting pipeline.
