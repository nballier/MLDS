

1 mars 9h-12h30 14h-17h30
22 mars  9h-12h30 14h-17h30

Les taggers probabilistes sont capables d'apprendre à prédire la catégorie morpho-syntaxique des mots, à partir de corpus d'entraînements. Plusieurs types d'annotations linguistiques sont possibles et plusieurs jeux d'étiquette (tagsets) ont été proposés pour des langues bien décrites comme l'anglais. Pour l'anglais, les jeux d'étiquettes implémentés confèrent des statuts différents aux réalisations possibles de that (Ballier et al, submitted). On s'intéressera ici à la distinction entre that relatif (The man that I saw) et le that des complétives nominales (the fact that I saw a man)  qui n'est distinguée que dans la version 8 de la CLAWS.


FRAMAPAD:
https://mypads2.framapad.org/mypads/?/mypads/group/mlds-1l2yes9bc/pad/view/mlds1-om1v190x

exposés:

- jeux d'étiquettes pour l'anglais et rappels sur l'annotation

CLAWS 5
http://ucrel.lancs.ac.uk/claws5tags.html
CLAWS 7
http://ucrel.lancs.ac.uk/claws7tags.html
CLAWS 8:
ucrel.lancs.ac.uk/claws8tags.pdf

UPenn tagset
https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html
Santorini, B. 1990. Part-of-speech tagging guidelines for the Penn Treebank Project. Technical report MS-CIS-90-47, Department of Computer and Information Science, University of Pennsylvania.

- complétives nominales et relatives: différences structurelles et recherche de features

- l'annotation et la réannotation avec Treetagger

Treetagger
https://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/

22 mars

Le parsing : CoreNLP, cleanNLP: l'annotation de la syntaxe par constituants (et l'analyse en dépendances)
(CoreNLP)
https://stanfordnlp.github.io/CoreNLP/demo.html
https://corenlp.run/

https://stanfordnlp.github.io/CoreNLP/

Manning, Christopher D., Mihai Surdeanu, John Bauer, Jenny Finkel, Steven J. Bethard, and David McClosky. 2014. The Stanford CoreNLP Natural Language Processing Toolkit In Proceedings of the 52nd Annual Meeting of the Association for Computational Linguistics: System Demonstrations, pp. 55-60.

coreNLP -> Stanza  https://github.com/stanfordnlp/stanza/


- l'annotation (et la ré-annotation) en analyse de dépendance avec UDpipe
les annotations de dépendance (UD)
https://universaldependencies.org/

TASK:  Chercher l'étiquette des relatives et des complétives nominales

- le modèle CONNL-X (CONNL-U) de présentation des données

Buchholz, Sabine, & Marsi, Erwin (2006, June). CoNLL-X shared task on multilingual dependency parsing. In Proceedings of the tenth conference on computational natural language learning (CoNLL-X) (pp. 149-164).


TASK:  Identification des colonnes et  l'annotation et la ré-annotation avec UDpipe

https://github.com/ufal/udpipe

implémentations : https://pypi.org/project/ufal.udpipe/

https://pypi.org/project/spacy-udpipe/

les modèles UD pour l'anglais: https://universaldependencies.org/

l'exemple du modèle GUM:
https://universaldependencies.org/treebanks/en_gum/index.html
TASK : dans le modèle partut : identifier les erreurs d'annotation

https://raw.githubusercontent.com/UniversalDependencies/UD_English-ParTUT/master/en_partut-ud-test.conllu

modèle GUM et autres modèles

évaluation de la qualité (evaluation campaign)

Wisniewski, G., & Yvon, F. (2019, June). How Bad are PoS Tagger in Cross-Corpora Settings? Evaluating Annotation Divergence in the UD Project. In 2019 Annual Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies (pp. 218-227).
https://hal.archives-ouvertes.fr/hal-02055137

outil de vérification
Wisniewski, G. (2018, May). Errator: a tool to help detect annotation errors in the universal dependencies project. In Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018).

Errator https://perso.limsi.fr/wisniews/errator/

BONUS:

- les complétives nominales zéro (plus the fact I'm a coward)

- l'incorpation du trait (feature) [+singulier] ou [+pluriel]

-feature engineering : ajouter des features sémantiques dans les noms : expérience avec la bibliothèque skweak de python, utiliser les fonction supervisées pour annoter les éléments pertinents. (ex. utiliser les fonctionnalités de gazetteer pour détecter les noms recteurs). 
https://github.com/NorskRegnesentral/skweak

l'approche machine learning : analyse en features:
- structuration du jeu de données (l'approche par dataset) : quelle information extraire? (Groupe 9)
- le feature engineering
- assigning more complex features. exemple avec that et d'autres réalisations (proforme) Gaillat et al. (2014)
https://www.researchgate.net/publication/266209855_Automated_classification_of_unexpected_uses_of_this_and_that_in_a_learner_corpus_of_English#fullTextFileContent

évaluation/projet étudiant

A partir de l'annotation du corpus Brown contenue dans la bibliothèque NLTK,  les étudiants procèderont

- à une classification des réalisations du that postnominal dans le Brown

- à un entraînement de Treetagger avec les étiquettes WPR pour le that relatif et CJT pour le that complétif. Ils évalueront la précision et le rappel de leur modèle.

- à partir de l'analyse en dépendance du corpus Brown, ils testeront l'annotation obtenue avec les différents modèles disponibles sur le github de UD et évalueront la qualité des modèles à l'aune de la distinction relative/complétive.

Your paper should follow the ACL template and style sheet for papers Style sheets (Latex, Word) are available here: http://acl2020.org/downloads/acl2020-templates.zip Upload your .zip file on the moodle, inluding the PDF describing your system, the text file including your examples of noun complement clauses and your code.
Explain who did what.  

Deadline de remise des travaux : 15 mai 2021 minuit.


PLAN-TYPE:
Introduction (deux structures : exemples, rappel des propriétés)
problématique N proposition

1. Travaux précédents
- jeux d'étiquettes (CLAWS8)
- Penn treebank
- UD (ccomp -> acl vs. acl:relcl)

2. Méthodes et outils
- Brown corpus (filtrage)
- méthode = réannotation et ré-entraînement
(même chose en UD)
- Treetagger: fonctions de réentraînement

3. Résultats
- baseline: Treetagger avec le fichier paramètre .par par défaut
- expérience réannotation partielle (précision)
- expérience : réannotation "maximale" (60% du Brown) (précision?)

4. Discussion
4.1 gain en précision ?
(graphe:  x: nombre d'exemples / y précision ) ?
[Si vous disposez de plusieurs sections du Brown (sinon coupez votre corpus d'annotation en deux ou en dix), faites l'expérience suivante: si vous réentraînez TreeTagger avec la moitié ou avec un corpus d'entraînement plus gros, quel est le gain en précision?
Vous pouvez faire figurer en x le nombre de tokens du corpus d'entraînement ou le nombre de that annotés.]



4.2.  surentrainement  (catégories du corpus Brown : press > anglais technique?)
4.3 features sous-estimés (pluriel / singulier) / that ou zéro ? / that adjacent ou pas ?

Conclusion / pistes de recherche

