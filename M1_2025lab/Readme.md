

## LABS 

#  Treetagger for POS-tagging:
For all the categories of *that*, run Treetagger with the test files. Report precision for each realisation. For instance, that as adverbs should be tagged as AVO (BNC.par, CLaws5 tagset) or RB (default parameter, Penn.par model, Penn Treebank tagset). 
Test the different testing files tags and report the precision for the different test sets.

bonus: compare performance of Penn and BNC models with Treetagger (bnc.par et penn.par).


# Retrain Treetagger   <br/>

## TIPS : example with French (In French)    <br/>
[example with French (In French)](https://pro.aiakide.net/cours/2022Annot/Corpus%20annotation%20-%20TD%206.pdf) <br/>


# ASSIGNMENT:

Retrain Treetagger with a specific tagset that distinguishes the different uses of *that*. Report precision and recall with the specific test datasets.

### C8 tagset [adapted]:(https://ucrel.lancs.ac.uk/claws8tags.pdf)   <br/>
WPR relative pronoun, "that"  <br/>
CST "that" (as conjunction for nouns, as in *the fact that*). Note that this tag in C7 subsumed both “that” as a complementizer and “that” as a relativizer  <br/>
CJT "that" as a conjunction for verbs (I think that you are right)    <br/>
DT singular determiner (e.g. "this", "that", "another")  <br/>
RB adverb  (it's not that difficult)   <br/>


For collaborative teams, explain in one paragraph who did what. Follow the CRediT attribution system 
 [doi:10.1087/20150211](https://www.researchgate.net/profile/Amy-Brand-2/publication/274098676_Beyond_authorship_Attribution_contribution_collaboration_and_credit/links/565b08c608aeafc2aac60656/Beyond-authorship-Attribution-contribution-collaboration-and-credit.pdf?__cf_chl_tk=oAqPOf76kxzKQ2Eo34enuDZpmKGvCijbSCoVQ5OYBrM-1736343622-1.0.1.1-SvCS95t3z1me8LVpJQkpRsN1e8PAQNTh7Yk5gjV1gqg) 

Your paper should follow the ACL template and style sheet for papers Style sheets (Latex, Word) are available here: http://acl2020.org/downloads/acl2020-templates.zip 

Upload your .zip file on  moodle, inluding the PDF describing your system, the text file including your examples of noun complement clauses and your code.


### Dépôt sur moodle
"IFHFBU41 Data Science avancée" pour les M1 en alternance  [IFHFBE40 Data science avancée](https://moodle.u-paris.fr/course/view.php?id=28636#section-1)

et "IFABY030 Data Science avancée" pour less [M1 en formation initiale](https://moodle.u-paris.fr/course/view.php?id=28339#section-0)



8 janvier  2025   9h-12h30 14h-17h30  <br>

15 janvier 2025  9h-12h30 14h-17h30

Les taggers probabilistes sont capables d'apprendre à prédire la catégorie morpho-syntaxique des mots, à partir de corpus d'entraînements. Plusieurs types d'annotations linguistiques sont possibles et plusieurs jeux d'étiquette (tagsets) ont été proposés pour des langues bien décrites comme l'anglais. Pour l'anglais, les jeux d'étiquettes implémentés confèrent des statuts différents aux réalisations possibles de *that* (Ballier et al, submitted). On s'intéressera ici à la distinction entre *that* relatif (*The man that I saw*) et le *that* des complétives nominales (*the fact that I saw a man*), qui n'est distinguée que dans la version 8 de la CLAWS. Le projet à réaliser pour l'évaluation consiste à re-éntraîner un tagger pour annoter la distintion *that* de complétive nominale (conjonction de subordination, CST) vs. *that* de relative (pronom, WPR) et d'analyser le rôle de la fréquence des *that* dans les corpus d'entraînements sur la précision (*accuracy*).


FRAMAPAD:
https://mypads2.framapad.org/mypads/?/mypads/group/mlds-1l2yes9bc/pad/view/mlds1-om1v190x


Présentation générale du NLP

exposés:
- jeux d'étiquettes pour l'anglais et rappels sur l'annotation

CLAWS 5 <br>
http://ucrel.lancs.ac.uk/claws5tags.html <br>
CLAWS 7 <br>
http://ucrel.lancs.ac.uk/claws7tags.html <br>
[CLAWS 8](https://ucrel.lancs.ac.uk/claws8tags.pdf) <br>


UPenn tagset
https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html
Santorini, B. 1990. Part-of-speech tagging guidelines for the Penn Treebank Project. Technical report MS-CIS-90-47, Department of Computer and Information Science, University of Pennsylvania.

- complétives nominales et relatives: différences structurelles et recherche de features

- l'annotation et la réannotation avec Treetagger

**Treetagger
https://www.cis.uni-muenchen.de/~schmid/tools/TreeTagger/


** 8 janvier 2025**
TreeTagger

** 15 janvier 2025**

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

**TASK**:  Chercher l'étiquette des relatives et des complétives nominales
- le modèle CONNL-X (CONNL-U) de présentation des données : comprendre les caractéristiques des annotations

Buchholz, Sabine, & Marsi, Erwin (2006, June). CoNLL-X shared task on multilingual dependency parsing. In Proceedings of the tenth conference on computational natural language learning (CoNLL-X) (pp. 149-164).


**TASK: ** Identification des colonnes et  l'annotation et la ré-annotation avec UDpipe

https://github.com/ufal/udpipe

implémentations : https://pypi.org/project/ufal.udpipe/

https://pypi.org/project/spacy-udpipe/

les modèles UD pour l'anglais: https://universaldependencies.org/

l'exemple du modèle GUM:
https://universaldependencies.org/treebanks/en_gum/index.html

TASK : dans le modèle partut : identifier les erreurs d'annotation
https://raw.githubusercontent.com/UniversalDependencies/UD_English-ParTUT/master/en_partut-ud-test.conllu



Remarque: pour l'évaluation de la qualité (_evaluation campaign_)
Wisniewski, G., & Yvon, F. (2019, June). How Bad are PoS Tagger in Cross-Corpora Settings? Evaluating Annotation Divergence in the UD Project. In 2019 Annual Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies (pp. 218-227).
https://hal.archives-ouvertes.fr/hal-02055137

### outil de vérification (pour info)
Wisniewski, G. (2018, May). Errator: a tool to help detect annotation errors in the universal dependencies project. In Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018).

Errator https://perso.limsi.fr/wisniews/errator/


Stanza , Spacy : analyse du Treebank d'entraînement.



## BONUS:
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

A partir de l'annotation des corpus présents dans les Treebanks et du Brown contenue dans la bibliothèque NLTK,  les étudiants procèderont
- à une classification des réalisations du that postnominal dans les Treebanks de référence

- à un entraînement de Treetagger avec les étiquettes WPR pour le that relatif, RO pour le that adverbial et CJT pour le _that_ complétif de verbe et CST pour le . Ils évalueront la précision et le rappel de leur modèle. (**question bonus**: annoter les réalisation de _that_ pronom (_I love that!_).

- à partir des l'analyse en dépendance du corpus Brown, ils testeront l'annotation obtenue avec les différents modèles disponibles sur le github de UD et évalueront la qualité des modèles à l'aune de la distinction relative/complétive.

- Ils évalueront le rôle de la taille des données d'entraînement pour les gains en précision pour l'annotation.
  
bonus : réannotation du that comme pronom (I love that).
A partir des corpus de tests, la précision est-elle la même selon les catégories? Produire une matrice de confusion des exemples.



Your paper should follow the ACL template and style sheet for papers Style sheets (Latex, Word) are available here: http://acl2020.org/downloads/acl2020-templates.zip Upload your .zip file on  moodle, including the PDF describing your system, the text file including your examples of noun complement clauses and your code.
Explain who did what in the paper.  


Follow standard recommendations  for plagiarism and generative AI. Indicate in your appendix the prompts you have used if you have 


**Deadline** de remise des travaux : 9 février 2025 minuit.


# PLAN-TYPE:
Introduction (deux structures : exemples, rappel des propriétés)
Explication de la problématique de la ré-annotation 
Bilan de votre exploration d'un Treebank (limites..., données extraites)


1. Travaux précédents sur l'analyse du that et sa réannotation
(use Google Scolar)
- jeux d'étiquettes (CLAWS8)
- Penn Treebank
- UD pour l'analyse des dépendances (ccomp -> acl vs. acl:relcl)


2. Méthodes et outils
- Treebank (extractions des exemples type présentts dans le Treebank)
- corpus synthétique si besoin 
- méthode = réannotation et ré-entraînement (donnez des exemples de *that* réannotés)
(optionnel : matrice de confusion annotation du corpus/étiquette réelle)
(même chose en UD)
- Treetagger: fonctions de réentraînement

3. Résultats
- baseline: Treetagger avec le fichier paramètre .par par défaut
- expérience réannotation partielle (précision du modèle réentraîner)
- expérience : réannotation "maximale" (corpus synthétique, Brown ré-annoté) 

4. Discussion <br>
4.1 gain en précision ? <br>
(graphe:  x: nombre d'exemples / y précision ) ?
[Si vous disposez de plusieurs sections du Brown (sinon coupez votre corpus d'annotation en deux ou en dix), faites l'expérience suivante: si vous réentraînez TreeTagger avec la moitié ou avec un corpus d'entraînement plus gros, quel est le gain en précision?
Vous pouvez faire figurer en x le nombre de tokens du corpus d'entraînement ou le nombre de that annotés. Avec les corpus synthétiques, comparez avec 100, 200, 500 phrases.]


4.2.  surentrainement  (catégories du corpus Brown : press > anglais technique)? <br>
Quelle conséquencee le ré-entraînement sur une seule catégorie produit?


4.3 features sous-estimés (pluriel / singulier) / that ou zéro ? / that adjacent ou pas ? <br>

optionnel : a-t-on de meilleurs résultats en cherchant avec UDpipe les relatives (acl:relcl) et les complétives (acl)? <br>
optionnel : a-t-on de meilleurs résultats si on ré-entraîne  les xpos en WPR et CST  pour les *that* avec UDpipe ? <br>


Conclusion / pistes de recherche

Annexe:
- carnet jupyter avec expérience reproductible.
- fichier(s) de réentraînement (exemples de phrases réannotées)
- prompts éventuels pour les corpus synthétiques.





