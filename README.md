# Vakyansh Open Source Models

## Pretrained Models

| Pretrained Model | Description | Architecture | Pretrained Hours          |  Logs |
|------------------|----------|----|---------|-----|
| [CLSRIL-23](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/CLSRIL-23.pt) | Cross Lingual Speech Representations for Indic Languages, Contains 10,000 hours of training data from 23 Indic Languages. <br> [Citation: https://arxiv.org/abs/2107.07402 ](https://arxiv.org/abs/2107.07402 ) | Base | 10,000               | [wandb](https://wandb.ai/harveenchadha/EKSTEP-PRETRAINING)|
| [hindi_pretrained_4kh](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/hindi_pretrained_4kh.pt) | Trained on 4200 hours of Hindi Data| Base |  4200             |  |
| [kannada_pretrained_1400h](https://storage.googleapis.com/vakyaansh-open-models/kannada/pretrained/kannada_pretrained_1400h.pt) | Trained on 1400 hours of Kannada data| XLSR | 1400             | |


<br>


## Finetuned Models (works on [v2-hydra](https://github.com/Open-Speech-EkStep/vakyansh-wav2vec2-experimentation/tree/v2-hydra) branch*)

| Language | Pretrained Model | Finetuned Model | Dictionary | Single Model for Inference | Finetuned Hours | 
|----|--------|----|-----|-------------------|-------|
| Hindi | CLSRIL-23 | [him_4200](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/him_4200.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/dict.ltr.txt ) | [hindi_infer](https://storage.googleapis.com/vakyansh-open-models/models/hindi/hi-IN/hindi_infer.pt) | 4200 h | 
| Indian English | CLSRIL-23 | [enm_700](https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/enm_700.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/dict.ltr.txt) | [english_infer]( https://storage.googleapis.com/vakyansh-open-models/models/english/en-IN/english_infer.pt ) | 700 h |
| Kannada | CLSRIL-23 | [knm_560](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/knm_560.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/dict.ltr.txt) | [kannada_infer](https://storage.googleapis.com/vakyansh-open-models/models/kannada/kn-IN/kannada_infer.pt ) | 560 h |
| Tamil | CLSRIL-23 | [tam_250](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/tam_250.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/dict.ltr.txt) | [tamil_infer](https://storage.googleapis.com/vakyansh-open-models/models/tamil/ta-IN/tamil_infer.pt ) | 250 h |
| Bengali | CLSRIL-23 | [bnm_200](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/bnm_200.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/dict.ltr.txt) | [bengali_infer](https://storage.googleapis.com/vakyansh-open-models/models/bengali/bn-IN/bengali_infer.pt ) | 200 h |
| Nepali | CLSRIL-23 | [nem_130](https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/nem_130.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/dict.ltr.txt) | [nepali_infer]( https://storage.googleapis.com/vakyansh-open-models/models/nepali/ne-IN/nepali_infer.pt ) | 130 h |
| Telugu | CLSRIL-23 | [tem_100](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/tem_100.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/dict.ltr.txt ) | [telugu_infer](https://storage.googleapis.com/vakyansh-open-models/models/telugu/te-IN/telugu_infer.pt ) | 100 h |
| Gujarati | CLSRIL-23 | [gum_100](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/gum_100.pt ) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/dict.ltr.txt ) | [gujarati_infer](https://storage.googleapis.com/vakyansh-open-models/models/gujarati/gu-IN/gujarati_infer.pt ) | 100 h |

*\*Note: All future models will be open sourced on v2-hydra branch*

<br>
<br>


## Finetuned Models (works on [v1](https://github.com/Open-Speech-EkStep/vakyansh-wav2vec2-experimentation/tree/v1) branch) [Depreciated]
| Language | Pretrained Model | Architecture | Finetuned Model | Single Model for Inference | Finetuned Hours | Dictionary |
|----|--------|----|-----|----|-------------------|-------|
| Hindi | hindi_pretrained_4kh | Base | [hindi_finetuned_4kh](https://storage.googleapis.com/vakyaansh-open-models/hindi/finetuned/hindi_finetuned_4kh.pt) | [hindi](https://storage.googleapis.com/vakyaansh-open-models/hindi/custom_model/hindi.pt) |  4200             | [dict](https://storage.googleapis.com/vakyaansh-open-models/hindi/dictionary/dict.ltr.txt) |
| Kannada | kannada_pretrained_1400h | XLSR | [kannada_finetuned_570h](https://storage.googleapis.com/vakyaansh-open-models/kannada/finetuned/kannada_finetuned_570h.pt) | [kannada](https://storage.googleapis.com/vakyaansh-open-models/kannada/custom_model/kannada_v2.pt)| 570             | [dict](https://storage.googleapis.com/vakyaansh-open-models/kannada/dictionary/dict.ltr.txt) |
| English | hindi_pretrained_4kh | Base | [english_finetuned_181h](https://storage.googleapis.com/vakyaansh-open-models/english/finetuned/english_finetuned_181h.pt) | [english](https://storage.googleapis.com/vakyaansh-open-models/english/custom_model/combined_model.pt) |181             | [dict](https://storage.googleapis.com/vakyaansh-open-models/english/dictionary/dict.ltr.txt) |
| Marathi | hindi_pretrained_4kh | Base | [marathi_finetuned_100h](https://storage.googleapis.com/vakyaansh-open-models/marathi/finetuned/marathi_finetuned_100h.pt) | - | 100             | [dict](https://storage.googleapis.com/vakyaansh-open-models/marathi/dictionary/dict.ltr.txt) |
| Odia | hindi_pretrained_4kh | Base |[odia_finetuned_100h](https://storage.googleapis.com/vakyaansh-open-models/odia/finetuned/odia_finetuned_100h.pt) | [odia](https://storage.googleapis.com/vakyaansh-open-models/odia/custom_model/odia_v1.pt) | 100             | [dict](https://storage.googleapis.com/vakyaansh-open-models/odia/dictionary/dict.ltr.txt) |
| Tamil | hindi_pretrained_4kh | Base |[tamil_finetuned_40h](https://storage.googleapis.com/vakyaansh-open-models/tamil/finetuned/tamil_finetuned_40h.pt) | [tamil](https://storage.googleapis.com/vakyaansh-open-models/tamil/custom_model/tamil.pt) | 40             | [dict](https://storage.googleapis.com/vakyaansh-open-models/tamil/dictionary/dict.ltr.txt) |
| Telugu | hindi_pretrained_4kh | Base |[telugu_finetuned_40h](https://storage.googleapis.com/vakyaansh-open-models/telugu/finetuned/telugu_finetuned_40h.pt) | [telugu](https://storage.googleapis.com/vakyaansh-open-models/telugu/custom_model/telugu.pt) | 40             | [dict](https://storage.googleapis.com/vakyaansh-open-models/telugu/dictionary/dict.ltr.txt) |
| Gujarati | hindi_pretrained_4kh | Base |[gujarati_finetuned_40h](https://storage.googleapis.com/vakyaansh-open-models/gujarati/finetuned/gujarati_finetuned_40h.pt) | [gujarati](https://storage.googleapis.com/vakyaansh-open-models/gujarati/custom_model/gujarati.pt) | 40             | [dict](https://storage.googleapis.com/vakyaansh-open-models/gujarati/dictionary/dict.ltr.txt) |


## Language Models

Data is taken from [AI For Bharat Corpus](https://indicnlp.ai4bharat.org/corpora/) but we do post processing by tokenizing and removing duplicates.

| Language | Type | Data | Sentences | Lexicon | LM |
|----|--------|---------|------|--|--------|
| Hindi | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/hindi/lm_data/hi_processed.txt) | 13M | [lexicon](https://storage.googleapis.com/vakyaansh-open-models/hindi/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/hindi/lm/lm.binary) |
| Kannada | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/hindi/lm_data/hi_processed.txt) | 21M | [lexicon](https://storage.googleapis.com/vakyaansh-open-models/kannada/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/kannada/lm/lm.binary) |
| English | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/english/lm_data/en_processed.txt) | 10M | [lexicon](https://storage.googleapis.com/vakyaansh-open-models/english/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/english/lm/lm.binary) |
| Marathi | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/marathi/lm_data/mr_processed.txt) | 22M | [lexicon](https://storage.googleapis.com/vakyaansh-open-models/marathi/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/marathi/lm/lm.binary) |
| Odia | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/odia/lm_data/od_processed.txt) | 0.36M | [lexicon](https://storage.googleapis.com/vakyaansh-open-models/odia/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/odia/lm/lm.binary) |
| Tamil | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/tamil/lm_data/ta_processed.txt) | 21M | [lexicon](https://storage.googleapis.com/vakyaansh-open-models/tamil/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/tamil/lm/lm.binary) |
| Telugu | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/telugu/lm_data/te_processed.txt) | 26M | [lexicon](https://storage.googleapis.com/vakyaansh-open-models/telugu/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/telugu/lm/lm.binary) |
| Gujarati | kenlm | [data](https://storage.googleapis.com/vakyaansh-open-models/gujarati/lm_data/gu_processed.txt) | 30M |[lexicon](https://storage.googleapis.com/vakyaansh-open-models/gujarati/lm/lexicon.lst) | [lm](https://storage.googleapis.com/vakyaansh-open-models/gujarati/lm/lm.binary) |

