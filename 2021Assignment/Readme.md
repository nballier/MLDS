# 2022 ASSIGNMENTS


Some of the tasks are taken from the REPROLANG 2020 workshop: Shared Task on the Reproduction of Research Results in Science and Technology of Language
Collocated with LREC 2020 12th Language Resources and Evaluation Conference. \
<https://lrec2020.lrec-conf.org/en/reprolang2020/>
"Participants are expected to obtain the data and tools for the reproduction from the information provided in the paper. Using the description of the experiment is part of the reproduction exercise."
 


## Deadline = March 7th midnight (2022)
Assignment : a replication study \
1- the docker with the system (if required, eg D.3) and the code  or executable code 'as is' on github \
2- A two-page paper summarizing your work (take more space if needed, 4 pages max). 


## Requirements
Your data and code should be encapsulated in a docker: see examples of similar requirements \
<https://lrec2020.lrec-conf.org/en/reprolang2020/submission/>

Your assignment must respect the requirements of a research paper (introduction, state of the art, presentation of your results, discussion and a reference section with the proper format), following a given paper template \
<https://lrec2022.lrec-conf.org/media/filer_public/16/8e/168e56e8-fb15-4213-bfbb-9e64de6b0bc9/lrec_2022_latex_template.zip>.
(LaTeX preferred, otherwise use Open Office or Word tempate <https://lrec2022.lrec-conf.org/media/filer_public/e0/7e/e07e434e-6ef0-4de7-86eb-93b28989f4c1/lrec_2022_word_template.dotx>.


**SUGGESTED OUTLINE** \
introduction \
state of the art \
summary of the replicated study  \
results  \
issues \
discussion  \
conclusion  \
acknowledgement: be explicit about how you split the work between members of the team  <br/>
Reference section <br/>
(Make sure you follow the recommended format for the bibliography).


## Task D.2: Language proficiency scoring
Vajjala, Sowmya, and Taraka Rama. 2018. “Experiments with Universal CEFR classifications”. In Proceedings of Thirteenth Workshop on Innovative Use of NLP for Building Educational Applications, pp. 147–153.
paper: <http://aclweb.org/anthology/W18-0515>  \
code:  <https://github.com/nishkalavallabhi/UniversalCEFRScoring>
data : <https://zenodo.org/record/1218081>
Major reproduction comparables: f-score values (tables 2, 3 and 4).

## Task D.3: Neural machine translation
Vanmassenhove, Eva, and Andy Way. 2018. “SuperNMT: Neural Machine Translation with Semantic Supersenses and Syntactic Supertags”. In Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics (ACL 2018), pp. 67–73. \
<http://aclweb.org/anthology/P18-3010>
Major reproduction comparables: BLEU scores (tables 1 and 2; plots in figures 2, 3 and 4).


# Replicating a paper in relation to Neural Translation

##  Evaluating Gender Bias in Machine Translation Gabriel Stanovsky, Noah A. Smith, and Luke Zettlemoyer, (ACL 2019) 
paper: <https://arxiv.org/abs/1906.00591> \
github:  <https://github.com/gabrielStanovsky/mt_gender> \

Major reproduction comparables: Table 2 and 3 and Figure 2 using DeepL \
<https://pypi.org/project/deep-translator/> 


## Reducing Gender Bias in Neural Machine Translation as a Domain Adaptation Problem (ACL 2020) 
paper : <https://arxiv.org/abs/2004.04498>
Major reproduction comparables : Table 2 for English/ French with Deepl and Google Translate
<https://pypi.org/project/deep-translator/> \
<https://github.com/DCSaunders/gender-debias>  


## Rico Sennrich, Barry Haddow, and Alexandra Birch. 2015. Improving neural machine translation models with monolingual data. arXiv preprint arXiv:1511.06709. 
<https://arxiv.org/abs/1511.06709>


## Vig, J. (2019). A multiscale visualization of attention in the transformer model.  
<https://arxiv.org/abs/1906.05714>  <br/>
<https://colab.research.google.com/drive/1YoJqS9cPGu3HL2_XExw3kCsRBtySQS2v?usp=sharing#scrollTo=nT4T5bdEt54v> <br/>
Réplication des visualisations des matrices d'attention pour les données anglaises de 
<https://github.com/gabrielStanovsky/mt_gender/blob/master/data/aggregates/en_pro.txt>
Observe-t-on des liens particuliers entre le pronom et son antécédent? <br/>
Pour quelle couche de neurones cela semble-t-il le plus flagrant? 

Vous chercherez à analyser les effets  des distracteurs, notamment dans le cas des relatives, pour des schémas de Wingrad  (cherchez d'autres exemples avec 'Winograd scheme challenge')  analysez les visualisations pour: <br/>
The city councilmen refused the demonstrators a permit because they [feared/advocated] violence.  <br/>
The choices of "feared" and "advocated" turn the schema into its two instances: <br/>
The city councilmen refused the demonstrators a permit because they feared violence. <br/>
The city councilmen refused the demonstrators a permit because they advocated violence. <br/> 

Analysez la référence du they avec la présence de distracteur:
The city councilmen refused the demonstrators who came with their trucks  a permit because they advocated violence. 
The city councilmen refused the demonstrators who came with their children  a permit because they advocated violence. 





## References
### Useful pointers from previous editions of the reprolang workshop: 
<http://4real.di.fc.ul.pt/> 4REAL Workshop : Workshop on Research Results Reproducibility and Resources Citation in Science and Technology of Language

### Proceedings of the 2020 REPROLANG edition :
<https://lrec2020.lrec-conf.org/en/reprolang2020/reprolang-accepted-papers/>


## MARKING SCHEME /20 
# paper /12  
clarity  \
understanding of the research question  <br/>
explicitness (explain why you can't get results or find different results)  <br/>
precision of results  
bibliographical conventions <br/>
respect of the original template 


# code / 8
executable docker \
quality of comments 

