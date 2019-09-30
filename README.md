# NorSentLex

## Overview

This repo contains a Norwegian sentiment lexicon of positive and negative words, semi-automatically created on the basis of the English lexicon compiled by Hu and Liu (2004). 

## Cite

When using this lexicon, please cite the following paper:

```
@InProceedings{BarSamOvr19,
  author = {Barnes, Jeremy and Touileb, Samia and {\O}vrelid, Lilja and Velldal, Erik},
  title = {Lexicon information in neural sentiment analysis: a multi-task learning approach},
  booktitle = {Proceedings of the 22nd Nordic Conference on Computational Linguistics},
  year = 2019,
  url = "https://www.aclweb.org/anthology/W19-6119/", 
  address = {Turku, Finland}
}
```
Code for replicating the experiments in the paper can be found here: https://github.com/ltgoslo/mtl_lex 

## Process 
We briefly describe the process of generating the lexicon(s) below, for further details see Barnes et al. (2019). 

The English lexicon of Hu and Liu (2004) was machine-translated and then manually inspected and corrected. If an English word had several senses that could be translated into different Norwegian words, these were manually added to the translations. All multi-word expressions were omitted, and only single-word translations have been included. Some words were also removed either because we found they did not fit into the positive or negative categories, or because we could not find an appropriate translation. We also removed all words listed as both positive and negative.

This process resulted in a Norwegian sentiment lexicon containing a collection of 3,917 negative and 1,601 positive words. Similarly to the English lexicon, the resulting Norwegian lexicon contains a mix of word classes and inflected forms. However, using the Norwegian full-form lexicon SCARRIE, we expanded the entries to include all inflected forms, resulting in a lexicon of 14,839 negative words and 6,103 positive words. Both versions of the lexicon are made avilable here.


## References: 

M. Hu and B. Liu  
_Mining and summarizing customer reviews_  
Proceedings of the 10th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining  
Seattle, USA  
2004 

J. Barnes, S. Touileb, L. Øvrelid and E. Velldal  
_Lexicon information in neural sentiment analysis: a multi-task learning approach_  
Proceedings of the 22nd Nordic Conference on Computational Linguistics  
Turku, Finland  
2019
URL: https://www.aclweb.org/anthology/W19-6119/
