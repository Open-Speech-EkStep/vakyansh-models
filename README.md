# Vakyansh Open Source Models

## Pretrained Models

| Pretrained Model | Description | Architecture | Pretrained Hours          |  Logs |
|------------------|----------|----|---------|-----|
| [hindi_pretrained_4kh](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/hindi_pretrained_4kh.pt) | Trained on 4200 hours of Hindi Data| Base |  4200             |  |
| [kannada_pretrained_1400h](https://storage.googleapis.com/vakyaansh-open-models/kannada/pretrained/kannada_pretrained_1400h.pt) | Trained on 1400 hours of Kannada data| XLSR | 1400             | |
| [CLSRIL-23](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/CLSRIL-23.pt) | Cross Lingual Speech Representations for Indic Languages, Contains 10,000 hours of training data from 23 Indic Languages | Base | 10,000               | [wandb](https://wandb.ai/harveenchadha/EKSTEP-PRETRAINING)|



## Finetuned Models
| Language | Pretrained Model | Architecture | Finetuned Model | Single Model for Inference | Finetuned Hours | Dictionary |
|----|--------|----|-----|----|-------------------|-------|
| Hindi | hindi_pretrained_4kh | Base | [hindi_finetuned_4kh](https://storage.googleapis.com/vakyaansh-open-models/hindi/finetuned/hindi_finetuned_4kh.pt) | [hindi_custom_model](https://storage.googleapis.com/vakyaansh-open-models/hindi/custom_model/hindi.pt) |  4200             | [dict](https://storage.googleapis.com/vakyaansh-open-models/hindi/dictionary/dict.ltr.txt) |
| Kannada | kannada_pretrained_1400h | XLSR | [kannada_finetuned_570h](https://storage.googleapis.com/vakyaansh-open-models/kannada/finetuned/kannada_finetuned_570h.pt) | [kannada_custom_model](https://storage.googleapis.com/vakyaansh-open-models/kannada/custom_model/kannada_v2.pt)| 570             | [dict](https://storage.googleapis.com/vakyaansh-open-models/kannada/dictionary/dict.ltr.txt) |
| English | hindi_pretrained_4kh | Base | [english_finetuned_181h](https://storage.googleapis.com/vakyaansh-open-models/english/finetuned/english_finetuned_181h.pt) | [english_custom_model](https://storage.googleapis.com/vakyaansh-open-models/english/custom_model/combined_model.pt) |181             | [dict](https://storage.googleapis.com/vakyaansh-open-models/english/dictionary/dict.ltr.txt) |
| Marathi | hindi_pretrained_4kh | Base | [marathi_finetuned_100h](https://storage.googleapis.com/vakyaansh-open-models/marathi/finetuned/marathi_finetuned_100h.pt) | - | 100             | [dict](https://storage.googleapis.com/vakyaansh-open-models/marathi/dictionary/dict.ltr.txt) |
| Odia | hindi_pretrained_4kh | Base |[odia_finetuned_100h](https://storage.googleapis.com/vakyaansh-open-models/odia/finetuned/odia_finetuned_100h.pt) | [odia_custom_model](https://storage.googleapis.com/vakyaansh-open-models/odia/custom_model/odia_v1.pt) | 100             | [dict](https://storage.googleapis.com/vakyaansh-open-models/odia/dictionary/dict.ltr.txt) |
| Tamil | hindi_pretrained_4kh | Base |[tamil_finetuned_40h](https://storage.googleapis.com/vakyaansh-open-models/tamil/finetuned/tamil_finetuned_40h.pt) | [tamil_custom_model](https://storage.googleapis.com/vakyaansh-open-models/tamil/custom_model/tamil.pt) | 40             | [dict](https://storage.googleapis.com/vakyaansh-open-models/tamil/dictionary/dict.ltr.txt) |
| Telugu | hindi_pretrained_4kh | Base |[telugu_finetuned_40h](https://storage.googleapis.com/vakyaansh-open-models/telugu/finetuned/telugu_finetuned_40h.pt) | [telugu_custom_model](https://storage.googleapis.com/vakyaansh-open-models/telugu/custom_model/telugu.pt) | 40             | [dict](https://storage.googleapis.com/vakyaansh-open-models/telugu/dictionary/dict.ltr.txt) |
| Gujarati | hindi_pretrained_4kh | Base |[gujarati_finetuned_40h](https://storage.googleapis.com/vakyaansh-open-models/gujarati/finetuned/gujarati_finetuned_40h.pt) | [gujarati_custom_model](https://storage.googleapis.com/vakyaansh-open-models/gujarati/custom_model/gujarati.pt) | 40             | [dict](https://storage.googleapis.com/vakyaansh-open-models/gujarati/dictionary/dict.ltr.txt) |


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

