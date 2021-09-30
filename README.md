# Vakyansh Open Source Models

## Pretrained Models

| Pretrained Model | Description | Architecture | Pretrained Hours          | 
|------------------|----------|----|---------|
| [CLSRIL-23](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/CLSRIL-23.pt) | Cross Lingual Speech Representations for Indic Languages, Contains 10,000 hours of training data from 23 Indic Languages. <br> [Citation: https://arxiv.org/abs/2107.07402 ](https://arxiv.org/abs/2107.07402 ) | Base | 10,000               | 
| [hindi_pretrained_4kh](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/hindi_pretrained_4kh.pt) | Trained on 4200 hours of Hindi Data| Base |  4200             |  
| [kannada_pretrained_1400h](https://storage.googleapis.com/vakyaansh-open-models/kannada/pretrained/kannada_pretrained_1400h.pt) | Trained on 1400 hours of Kannada data| XLSR | 1400 | 


<br>


## Finetuned Models (works on [v2-hydra](https://github.com/Open-Speech-EkStep/vakyansh-wav2vec2-experimentation/tree/v2-hydra) branch*)

| Language | Pretrained Model | Finetuned Model | Dictionary | Single Model for Inference | Finetuned Hours | TS model |
|----|--------|----|-----|-------------------|-------|---|
| Hindi | CLSRIL-23 | [him_4200](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/him_4200.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/dict.ltr.txt ) | [hindi_infer](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/hindi_infer.pt) | 4200 h | [hindi_ts](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/vakyansh-wav2vec2-hindi-him-4200_quant.pt)
| Indian English | CLSRIL-23 | [enm_700](https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/enm_700.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/dict.ltr.txt) | [english_infer]( https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/english_infer.pt ) | 700 h | [english_ts](https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/vakyansh-wav2vec2-indian-english-enm-700_quant.pt)
| Kannada | CLSRIL-23 | [knm_560](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/knm_560.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/dict.ltr.txt) | [kannada_infer](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/kannada_infer.pt ) | 560 h | [kannada_ts](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/vakyansh-wav2vec2-kannada-knm-560_quant.pt)
| Tamil | CLSRIL-23 | [tam_250](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/tam_250.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/dict.ltr.txt) | [tamil_infer](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/tamil_infer.pt ) | 250 h |  [tamil_ts](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/vakyansh-wav2vec2-tamil-tam-250_quant.pt)
| Bengali | CLSRIL-23 | [bnm_200](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/bnm_200.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/dict.ltr.txt) | [bengali_infer](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/bengali_infer.pt ) | 200 h | [bengali_ts](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/vakyansh-wav2vec2-bengali-bnm-200_quant.pt) |
| Nepali | CLSRIL-23 | [nem_130](https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/nem_130.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/dict.ltr.txt) | [nepali_infer]( https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/nepali_infer.pt ) | 130 h | [nepali_ts](https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/vakyansh-wav2vec2-nepali-nem-130_quant.pt)
| Telugu | CLSRIL-23 | [tem_100](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/tem_100.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/dict.ltr.txt ) | [telugu_infer](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/telugu_infer.pt ) | 100 h | [telugu_ts](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/vakyansh-wav2vec2-telugu-tem-100_quant.pt)
| Gujarati | CLSRIL-23 | [gum_100](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/gum_100.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/dict.ltr.txt ) | [gujarati_infer](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/gujarati_infer.pt ) | 100 h | [gujarati_ts](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/vakyansh-wav2vec2-gujarati-gnm-100_quant.pt)
| Marathi | CLSRIL-23 | [mrm_100](https://storage.googleapis.com/vakyansh-open-models/models/marathi/mr-IN/mrm_100.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/marathi/mr-IN/dict.ltr.txt) |  [marathi_infer](https://storage.googleapis.com/vakyansh-open-models/models/marathi/mr-IN/marathi_infer.pt) | 100 h | 
| Odia | CLSRIL-23 | [orm_100](https://storage.googleapis.com/vakyansh-open-models/models/odia/or-IN/orm_100.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/odia/or-IN/dict.ltr.txt) | [odia_infer](https://storage.googleapis.com/vakyansh-open-models/models/odia/or-IN/odia_infer.pt) | 100 h | 
| Sanskrit | CLSRIL-23 | [sam_60](https://storage.googleapis.com/vakyansh-open-models/models/sanskrit/sa-IN/sam_60.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/sanskrit/sa-IN/dict.ltr.txt) | [sanskrit_infer](https://storage.googleapis.com/vakyansh-open-models/models/sanskrit/sa-IN/sanskrit_infer.pt) | 60 h | 
| Maithili | CLSRIL-23 | [maim_50](https://storage.googleapis.com/vakyansh-open-models/models/maithili/mai-IN/maim_50h.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/maithili/mai-IN/dict.ltr.txt) | [maithili_infer](https://storage.googleapis.com/vakyansh-open-models/models/maithili/mai-IN/maithili_infer.pt) | 50 h | 
| Urdu | CLSRIL-23 | [urm_60h](https://storage.googleapis.com/vakyansh-open-models/models/urdu/ur-IN/urm_60h.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/urdu/ur-IN/dict.ltr.txt) | [urdu_infer](https://storage.googleapis.com/vakyansh-open-models/models/urdu/ur-IN/urm_infer.pt) | 60h |
| Punjabi | CLSRIL-23 | [pam_10h](https://storage.googleapis.com/vakyansh-open-models/models/punjabi/pa-IN/pam_10h.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/punjabi/pa-IN/dict.ltr.txt) | [punjabi_infer](https://storage.googleapis.com/vakyansh-open-models/models/punjabi/pa-IN/punjabi_infer.pt) |  10 h |
| Dogri | CLSRIL-23 | [doi_55h](https://storage.googleapis.com/vakyansh-open-models/models/dogri/doi-IN/doim_55h.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/dogri/doi-IN/dict.ltr.txt) | [dogri_infer](https://storage.googleapis.com/vakyansh-open-models/models/dogri/doi-IN/dogri_infer.pt) | 55 h |
| Malayalam | CLSRIL-23 | [mlm_8h](https://storage.googleapis.com/vakyansh-open-models/models/malayalam/ml-IN/mlm_8h.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/malayalam/ml-IN/dict.ltr.txt) | [malayalam_infer](https://storage.googleapis.com/vakyansh-open-models/models/malayalam/ml-IN/malayalam_infer.pt) | 8 h |
| Bhojpuri | CLSRIL-23 | [bhom_60h](https://storage.googleapis.com/vakyansh-open-models/models/bhojpuri/bho-IN/bhom_60h.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/bhojpuri/bho-IN/dict.ltr.txt) | [bhojpuri_infer](https://storage.googleapis.com/vakyansh-open-models/models/bhojpuri/bho-IN/bhojpuri_infer.pt) | 60 h |
| Rajasthani | CLSRIL-23 | [raj_45h](https://storage.googleapis.com/vakyansh-open-models/models/rajasthani/raj-IN/raj_45h.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/rajasthani/raj-IN/dict.ltr.txt) | [rajasthani_infer](https://storage.googleapis.com/vakyansh-open-models/models/rajasthani/raj-IN/rajasthani_infer.pt) | 45 h |

*\*Note: All future models will be open sourced on v2-hydra branch*



## Language Models

Data is taken from [AI For Bharat Corpus](https://indicnlp.ai4bharat.org/corpora/) but we do post processing by tokenizing and removing duplicates.

| Language | Type | Lexicon | LM |
|----|--------|---------|------|
| Hindi | kenlm 5-gram | [hindi_lexicon]( https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/lexicon.lst ) | [hindi_lm](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/lm.binary) |
| Indian English | kenlm 5-gram | [english_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/lexicon.lst ) | [english_lm](https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/lm.binary) |
| Kannada | kenlm 5-gram | [kannada_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/lexicon.lst) | [kannada_lm](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/lm.binary ) |
| Tamil | kenlm 5-gram | [tamil_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/lexicon.lst) | [tamil_lm](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/lm.binary) | 
| Bengali | kenlm 5-gram | [bengali_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/lexicon.lst) | [bengali_lm](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/lm.binary ) |
| Nepali | kenlm 5-gram | [nepali_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/lexicon.lst ) | [nepali_lm](https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/lm.binary ) |
| Telugu | kenlm 5-gram | [telugu_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/lexicon.lst) | [telugu_lm](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/lm.binary) |
| Gujarati | kenlm 5-gram | [gujarati_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/lexicon.lst ) | [gujarati_lm](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/lm.binary) | 
| Marathi | kenlm 5-gram | [marathi_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/marathi/mr-IN/lexicon.lst) | [marathi_lm](https://storage.googleapis.com/vakyansh-open-models/models/marathi/mr-IN/lm.binary) |
| Odia | kenlm 5-gram | [odia_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/odia/or-IN/lexicon.lst) | [odia_lm](https://storage.googleapis.com/vakyansh-open-models/models/odia/or-IN/lm.binary) | 
| Sanskrit | kenlm 5-gram | [sanskrit_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/sanskrit/sa-IN/lexicon.lst) | [sanskrit_lm](https://storage.googleapis.com/vakyansh-open-models/models/sanskrit/sa-IN/lm.binary)
| Maithili | kenlm 5-gram | [maithili_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/maithili/mai-IN/lexicon.lst) | [maithili_lm](https://storage.googleapis.com/vakyansh-open-models/models/maithili/mai-IN/lm.binary)
| Urdu | kenlm 5-gram | [urdu_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/urdu/ur-IN/lexicon.lst) | [urdu_lm](https://storage.googleapis.com/vakyansh-open-models/models/urdu/ur-IN/lm.binary)
| Punjabi | kenlm 5-gram | [punjabi_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/punjabi/pa-IN/lexicon.lst) | [punjabi_lm](https://storage.googleapis.com/vakyansh-open-models/models/punjabi/pa-IN/lm.binary)
| Dogri | kenlm 5-gram | [dogri_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/dogri/doi-IN/lexicon.lst) | [dogri_lm](https://storage.googleapis.com/vakyansh-open-models/models/dogri/doi-IN/lm.binary)
| Malayalam | kenlm 5-gram | [malayalam_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/malayalam/ml-IN/lexicon.lst) | [malayalam_lm](https://storage.googleapis.com/vakyansh-open-models/models/malayalam/ml-IN/lm.binary)
| Bhojpuri | kenlm 5-gram | [bhojpuri_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/bhojpuri/bho-IN/lexicon.lst) | [bhojpuri_lm](https://storage.googleapis.com/vakyansh-open-models/models/bhojpuri/bho-IN/lm.binary)
| Rajasthani | kenlm 5-gram | [rajasthani_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/rajasthani/raj-IN/lexicon.lst) | [rajasthani_lm](https://storage.googleapis.com/vakyansh-open-models/models/rajasthani/raj-IN/lm.binary)



## Domain Specific Language Models
| Language | Type | Domain | Lexicon | LM |
|----|--------|---------|------|---|
| English | kenlm 5-gram | Biomedical | [bio_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/english/bio-lm/lexicon.lst ) | [bio_lm](https://storage.googleapis.com/vakyansh-open-models/models/english/bio-lm/lm.binary )

<br>
<br>

<hr>

