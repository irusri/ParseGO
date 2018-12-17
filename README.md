# ParseGO
Parse Gene Ontology into tab delimited text file.

First download the OBO file from http://geneontology.org/page/download-ontology. Next run the following command.

<pre>
python ParseGO.py go.obo output_file
</pre>
<pre>
$ head go.obo
format-version: 1.2
data-version: releases/2018-12-17
subsetdef: gocheck_do_not_annotate "Term not to be used for direct annotation"
subsetdef: gocheck_do_not_manually_annotate "Term not to be used for direct manual annotation"
subsetdef: goslim_agr "AGR slim"
subsetdef: goslim_aspergillus "Aspergillus GO slim"
subsetdef: goslim_candida "Candida GO slim"
subsetdef: goslim_chembl "ChEMBL protein targets summary"
subsetdef: goslim_flybase_ribbon "FlyBase Drosophila GO ribbon slim"
subsetdef: goslim_generic "Generic GO slim"
</pre>
<pre>
$ head output_file
go_id	description	name_space
GO:0000001	mitochondrion inheritance	biological_process
GO:0000002	mitochondrial genome maintenance	biological_process
GO:0000003	reproduction	biological_process
GO:0019952	reproduction	biological_process
GO:0050876	reproduction	biological_process
GO:0000005	obsolete ribosomal chaperone activity	molecular_function
GO:0000006	high-affinity zinc transmembrane transporter activity	molecular_function
</pre>

