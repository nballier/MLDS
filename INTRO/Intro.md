**De la linguistique très outillée à la science des données des données linguistique**



Approche stratificationnelle de la linguistique : bilan de grandes approches automatiques et exemples de traitements/modélisation de jeux de données 



STRATA:  from domain to tools



AIMS:
1. culture linguistique
2. présentation d'outils de production de données
3. Quelques exemples de traitement de données (feature engineering)


1. phonétique :
thèse d'Adrien Méli
A longitudinal study of the oral properties of the French-English interlanguage A quantitative approach of the acquisition of the /I/-/i:/ and /U/-/u:/ contrast
par Adrien Meli (2018)


data collection:
http://mapage.noos.fr/admeli/poznan/#1
Vowel acquisition:
http://mapage.noos.fr/admeli/pac2015/
k-nn analysis for  i:/I (Méli & Ballier , accepted)
lda and and native/non-native speech discrimination
neural nets with .WAV files


2. phonologie : l'analyse de la syllabe
Seattle talk
Timbl and the LPD dataset


CMU 
http://www.speech.cs.cmu.edu/cgi-bin/cmudict
latest version in the SPHINX environment (for text-to speech with American Pronunciation:
http://svn.code.sf.net/p/cmusphinx/code/trunk/cmudict/cmudict-0.7b
SPHINX on githib: https://github.com/cmusphinx/cmudict

As explained on the website,
http://www.speech.cs.cmu.edu/cgi-bin/cmudict
the "phoneme set" is based on ARPABET, see the CMUPhonemeSet.txt file for conversions.

The latest CMU version can be downloaded from 
http://svn.code.sf.net/p/cmusphinx/code/trunk/cmudict/cmudict-0.7b

The data with syllables http://webdocs.cs.ualberta.ca/~kondrak/cmudict/cmudict.rep
is based on the CELEX syllable boundaries (not a good idea-NB) as explained in Bartlett et al. 2009.
Susan Bartlett, Grzegorz Kondrak and Colin Cherry (2009) 
On the Syllabification of Phonemes.NAACL-HLT 2009.




TiMIT for speech correlates and ML techniques for correlates of syllable boundaries 


3. morphologie 
concaténative / non-concaténative
3.0  Granada Talk: morphology
3.1 les suffixes dans les dictionnaires orthoépistes du 18e siècle
3.2 Treetagger et l'évolution du lexique (obsolete)
3.3 La lexicologie vs. la lexicographie du 18e siècle
Walker versus Sheridan
https://nbviewer.jupyter.org/urls/gitlab.huma-num.fr/mshs-poitiers/forellis/dicodiachro/raw/master/Buchanan_eng.ipynb?flush_cache=true
https://nbviewer.jupyter.org/urls/gitlab.huma-num.fr/mshs-poitiers/forellis/dicodiachro/raw/master/Buchanan-Walker_Exploration-Syneresis.ipynb?flush_cache=true
(Duchet et al., submitted)


3.4 l'analyse de l'amalgamation
Caractérisation d'un jeu de données en cours   

4. complexité lexicale et syntaxique:
classifications d'appenants (Lisson & Ballier 2019) 
https://discours.revues.org/


5. The CAP2018 challenge 
5.1. producing the dataset
http://cap2018.litislab.fr/competition.html
5.2 The winner
Balikasg https://arxiv.org/abs/1809.08935

5.3. syntactic metrics : Arnold et al. 2018 
https://arxiv.org/abs/1806.11099

5.4 Take home messages : (Ballier et al. Submitted)  

5.5 enriching the EFCAMDAT dataset : the PHC Ulysses 2019 project
http://www.clillac-arp.univ-paris-diderot.fr/projets/ulysse2019

Sample dataset with metadata
https://github.com/nballier/RforCorpusLinguists/blob/master/CELVA.Sp_286.csv

-> ELTAL submission
CTAP and TAALES linguistic tools
https://www.linguisticanalysistools.org/
CTAP: http://ctapweb.com/

6. discours 
Um and Uh, and the expression of stance in conversational speech, par Esther Le Grézause sous la direction de Nicolas Ballier et de Richard Wright. - Sorbonne Paris Cité, 
http://theses.md.univ-paris-diderot.fr/Le_Grezauze_Esther_2_va_20170523.pdf

7. semantics : Word embeddings and student levels??


8. The core NLP suite 
NER
coreference analysis
Sentiment Analysis


9. pragmatics/opinion mining (CBL)


10. Keylogs : process mining and learner analytics (Ballier & Gaillat 1209) 


