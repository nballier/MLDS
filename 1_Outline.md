# NLP CLASSES for MLDS STUDENTS FEBRUARY 2020 : PROVISIONAL PROGRAMME

Doc for MLSD students Initial session : Feb 7, 9h-17h30, Salle 704J, Paris Descartes, rue des Saint Pères.
    Outline of the talk : DataTalkSummary.txt
    revision: the strata of linguistics (from sound to meaning): STRATA.PDF
    dataset: the CMU dictionary
    restitution de la compétition CAp2018 : CAp2018-Competition.pdf

MLDS : 07/02 
An introduction to ML approaches to linguistics
- the stratificational model and some of its NLP implementations
- SPPAS : settig up an aligner : learning how to annotated data for supervised learning with speech data
(other aligners and python library)
- Praat the standard software for phonetic analysis
- A crash course to computational morphology
DRILL / RQ: BPE versus chipmunk
The new frontier : non-concatenative morphology
Morphological matrices

07/02 PM 
Neural Translation : some research questions and useful papers
- a great survey paper (80p)
- our method: input/process/output
- the benefit of annotated data
- challenges : the actual competition
- the assignment : 



## Feb 07,2020

###  AM:  NLP, tools, tasks and libraries: a general introduction
This intro talk is meant as a reminder of the different strata of linguistics, from phonetics to pragmatics, covering the main linguistic notions and some of their electronic correlates.  

#### From sound to meaning : a reminder of main linguistic notions and NLP tools

#### the stratificational model 
PDF

### PM 

#### 1. dealing with sound: the old school approach
Machine learning with annotated sound files
aligners : the case of SPPAS

#### Some NLP tools for sound :  an introduction
https://deepmind.com/blog/article/wavenet-generative-model-raw-audio

##### VGGISh google app
the Visual geometric analysis
https://github.com/tensorflow/models/tree/master/research/audioset/vggish

##### classification 
https://github.com/harritaylor/torchvggish
S. Hershey et al., ‘CNN Architectures for Large-Scale Audio Classification’,\ in International Conference on Acoustics, Speech and Signal Processing (ICASSP),2017\ Available: https://arxiv.org/abs/1609.09430, https://ai.google/research/pubs/pub45611

#####Deepmind 
https://deepmind.com/blog/article/wavenet-generative-model-raw-audio

###### TACOTRON


## Feb 14, 2020 

### AM The CAp2018 competition: dataset, NLP-based features and learner data
tools for complexity analysis: the  linguistictools.org family of tools

hands-on session on approaches to complexity 

11H: skype with Patrick: the NUCLE corpus

### PM CEFR prediction : the Ulysses 2019 research project 
http://www.clillac-arp.univ-paris-diderot.fr/projets/ulysse2019
 
 
#### Language proficiency scoring : the BEA Workshop
Proceedings of the Thirteenth Workshop on Innovative Use of NLP for Building Educational Applications

#### Vajjala, Sowmya, and Taraka Rama. 2018. “Experiments with Universal CEFR classifications”. In Proceedings of Thirteenth Workshop on Innovative Use of NLP for Building Educational Applications, pp. 147–153.
http://aclweb.org/anthology/W18-0515
Major reproduction comparables: f-score values (tables 2, 3 and 4).
https://github.com/nishkalavallabhi/UniversalCEFRScoring

####  BEA2019 TASK : issues and details  (the proposed project)

####  your assignment on NMT

