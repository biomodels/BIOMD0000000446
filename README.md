# BIOMD0000000446: MODEL1302180000

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000446.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000446.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000446 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


Erguler2013 - Unfolded protein stress response

The model investigates the mechanism by which UPR (unfolded protein response)
outcome switches between survival and death.

This model is described in the article:

[A mathematical model of the unfolded protein stress response reveals the
decision mechanism for recovery, adaptation and
apoptosis.](http://identifiers.org/pubmed/23433609)

Erguler K, Pieri M, Deltas C.

BMC Syst Biol. 2013 Feb 21;7(1):16.

Abstract:

BACKGROUND: The unfolded protein response (UPR) is a major signalling cascade
acting in the quality control ofprotein folding in the endoplasmic reticulum
(ER). The cascade is known to play an accessory rolein a range of genetic and
environmental disorders including neurodegenerative and
cardiovasculardiseases, diabetes and kidney diseases. The three major
receptors of the ER stress involved withthe UPR, i.e. IRE1a, PERK and ATF6,
signal through a complex web of pathways to convey anappropriate response. The
emerging behaviour ranges from adaptive to maladaptive depending on
theseverity of unfolded protein accumulation in the ER; however, the decision
mechanism for the switchand its timing have so far been poorly understood.

RESULTS: Here, we propose a mechanism by which the UPR outcome switches
between survival and death.We compose a mathematical model integrating the
three signalling branches, and perform a comprehensivebifurcation analysis to
investigate possible responses to stimuli. The analysis reveals threedistinct
states of behaviour, low, high and intermediate activity, associated with
stress adaptation, tolerance,and the initiation of apoptosis. The decision to
adapt or destruct can, therefore, be understoodas a dynamic process where the
balance between the stress and the folding capacity of the ER playsa pivotal
role in managing the delivery of the most appropriate response. The model
demonstratesfor the first time that the UPR is capable of generating
oscillations in translation attenuation and theapoptotic signals, and this is
supplemented with a Bayesian sensitivity analysis identifying a set
ofparameters controlling this behaviour.

CONCLUSIONS: This work contributes largely to the understanding of one of the
most ubiquitous signalling pathwaysinvolved in protein folding quality control
in the metazoan ER. The insights gained have direct consequenceson the
management of many UPR-related diseases, revealing, in addition, an extended
listof candidate disease modifiers. Demonstration of stress adaptation sheds
light to how preconditioningmight be beneficial in manifesting the UPR outcome
to prevent untimely apoptosis, and paves the wayto novel approaches for the
treatment of many UPR-related conditions.

In the paper, PERKA refers to the amount of phosphorylated PERK monomer.
However, it refers to the active complex in the model. The complex with the
model parameterization is formed of 4 monomers (n=4). So, the value of PERKA
should be multiplied by 4, in order to generate the figures in the paper (eg.
Figure 12).

An additional parameter (tmr=10)) is used in the model. This parameter is not
mentioned in the paper. The model values of kf(=10) and kr(=1) are not
consistent with that of the paper (kf=100, kr=10, in the paper). However, this
is corrected by the introduction of "tmr" in the model, which is multiplied
with kf and kr to get the resulting values.

The term "tmr" was missing in the kinetic laws of the reactions reu7 and reu8,
in the original model. This has been corrected as per the author's request.

This model is hosted on [BioModels Database](http://www.ebi.ac.uk/biomodels/)
and identified by:
[MODEL1302180000](http://identifiers.org/biomodels.db/MODEL1302180000) .

To cite BioModels Database, please use: [BioModels Database: An enhanced,
curated and annotated resource for published quantitative kinetic
models](http://identifiers.org/pubmed/20587024) .

To the extent possible under law, all copyright and related or neighbouring
rights to this encoded model have been dedicated to the public domain
worldwide. Please refer to [CC0 Public Domain
Dedication](http://creativecommons.org/publicdomain/zero/1.0/) for more
information.


