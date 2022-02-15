# Vakyansh Open Source Models


## TTS Models ([Repo](https://github.com/Open-Speech-EkStep/vakyansh-tts))
Below models are trained using [Glow TTS](https://github.com/jaywalnut310/glow-tts) and [hifi GAN](https://github.com/jik876/hifi-gan) combination. 

| Language | Gender | glow ckpt | hifi-gan ckpt | 
| ------- | ----- | ---- | ------------ |
| Hindi | Female | [voice_0_glow](https://storage.googleapis.com/vakyansh-open-models/tts/hindi/hi-IN/female_voice_0/glow.zip) | [voice_0_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/hindi/hi-IN/female_voice_0/hifi.zip) |
| Hindi | Male | [voice_1_glow](https://storage.googleapis.com/vakyansh-open-models/tts/hindi/hi-IN/male_voice_1/glow.zip) | [voice_1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/hindi/hi-IN/male_voice_1/hifi.zip) |
| Kannada | Female | [voice_0_glow](https://storage.googleapis.com/vakyansh-open-models/tts/kannada/kn-IN/female_voice_0/fe_glow.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/kannada/kn-IN/ma_fe_hifi/ma_fe_hifi.zip) |
| Kannada | Male | [voice_1_glow](https://storage.googleapis.com/vakyansh-open-models/tts/kannada/kn-IN/male_voice_1/ma_glow.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/kannada/kn-IN/ma_fe_hifi/ma_fe_hifi.zip)  |
| Tamil | Female | [voice_0_glow](https://storage.googleapis.com/vakyansh-open-models/tts/tamil/ta-IN/female_voice_0/glow.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/tamil/ta-IN/ma_fe_hifi/hifi.zip) |
| Tamil | Male | [voice_1_glow](https://storage.googleapis.com/vakyansh-open-models/tts/tamil/ta-IN/male_voice_1/glow.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/tamil/ta-IN/ma_fe_hifi/hifi.zip)  |
| Telugu | Female | [voice_0_glow](https://storage.googleapis.com/vakyansh-open-models/tts/telugu/te-IN/female_voice_0/glow.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/telugu/te-IN/ma_fe_hifi/hifi.zip) |
| Telugu | Male | [voice_1_glow](https://storage.googleapis.com/vakyansh-open-models/tts/telugu/te-IN/male_voice_1/glow.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/telugu/te-IN/ma_fe_hifi/hifi.zip)  |
| Odia | Female | [voice_0_glow](https://storage.googleapis.com/vakyansh-open-models/tts/odia/or-IN/female_voice_0/glow.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/odia/or-IN/ma_fe_hifi/hifi.zip) |
| Odia | Male | [voice_1_glow](https://storage.googleapis.com/vakyansh-open-models/tts/odia/or-IN/ma_fe_hifi/hifi.zip) | [voice_0_and 1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/odia/or-IN/ma_fe_hifi/hifi.zip)  |
| Malayalam | Female | [voice_0_glow](https://storage.googleapis.com/vakyansh-open-models/tts/malayalam/ml-IN/female_voice_0/glow.zip) | [voice_0_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/malayalam/ml-IN/female_voice_0/hifi.zip) |
| Malayalam | Male | [voice_1_glow](https://storage.googleapis.com/vakyansh-open-models/tts/malayalam/ml-IN/male_voice_1/glow.zip) | [voice_1_hifi](https://storage.googleapis.com/vakyansh-open-models/tts/malayalam/ml-IN/male_voice_1/hifi.zip) |

Credits: We thanks IITM for providing open sourcing Indic-TTS dataset<br>
[Link](https://www.iitm.ac.in/donlab/tts/database.php)

## Pretrained ASR Models


| Pretrained Model | Description | Architecture | Pretrained Hours |
|------------------|----------|----|---------|
| [CLSRIL-23](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/CLSRIL-23.pt) | Cross Lingual Speech Representations for Indic Languages, Contains 10,000 hours of training data from 23 Indic Languages. <br> [Citation: https://arxiv.org/abs/2107.07402 ](https://arxiv.org/abs/2107.07402 ) | Base | 10,000               | 
| [hindi_pretrained_4kh](https://storage.googleapis.com/vakyaansh-open-models/hindi/pretrained/hindi_pretrained_4kh.pt) | Trained on 4200 hours of Hindi Data| Base |  4200             |  
| [kannada_pretrained_1400h](https://storage.googleapis.com/vakyaansh-open-models/kannada/pretrained/kannada_pretrained_1400h.pt) | Trained on 1400 hours of Kannada data| XLSR | 1400             | 


<br>


## Finetuned ASR Models (works on [v2-hydra](https://github.com/Open-Speech-EkStep/vakyansh-wav2vec2-experimentation/tree/v2-hydra) branch*)

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
| Assamese | CLSRIL-23 | [asm_8h](https://storage.googleapis.com/vakyansh-open-models/models/assamese/asm_8.pt) | [dict](https://storage.googleapis.com/vakyansh-open-models/models/assamese/dict.ltr.txt) | [assamese_infer](https://storage.googleapis.com/vakyansh-open-models/models/assamese/assamese_infer.pt) | 8 h |




## Language Models (Works with Finetuned ASR Models)

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
| Assamese | kenlm 5-gram | [assamese_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/assamese/lexicon.lst) | [assamese_lm](https://storage.googleapis.com/vakyansh-open-models/models/assamese/lm.binary) 

## Domain Specific Language Models
| Language | Type | Domain | Lexicon | LM |
|----|--------|---------|------|---|
| English | kenlm 5-gram | Biomedical | [bio_lexicon](https://storage.googleapis.com/vakyansh-open-models/models/english/bio-lm/lexicon.lst ) | [bio_lm](https://storage.googleapis.com/vakyansh-open-models/models/english/bio-lm/lm.binary )


## Punctuation Models
| Language | Model | Data | 
|----------|-------|-------|
| Hindi | [hi.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/hi.zip)| [hindi_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/hindi.zip)|
| Assamese | [as.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/as.zip)| [assamese_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/assamese.zip) |
| Bengali | [bn.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/bn.zip)| [bengali_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/bengali.zip)|
| Gujarati | [gu.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/gu.zip)| [gujarati_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/gujarati.zip)|
| Kannada | [kn.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/kn.zip)| [kannada_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/kannada.zip)|
| Malayalam | [ml.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/ml.zip)| [malayalam_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/malayalam.zip)|
| Marathi | [mr.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/mr.zip)| [marathi_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/marathi.zip)|
| Odia | [or.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/or.zip)| [odia_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/oria.zip)|
| Punjabi | [pa.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/pa.zip)| [punjabi_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/punjabi.zip)|
| Tamil | [ta.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/ta.zip)| [tamil_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/tamil.zip)|
| Telugu | [te.zip](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/te.zip)| [telugu_data](https://storage.googleapis.com/vakyaansh-open-models/punctuation_models/telugu.zip)|

Credits for punctuation data - [IndicCorp AI4Bharat](https://indicnlp.ai4bharat.org/corpora/)

<br>

## Citation 


If you use any of our resources, please cite the following article. 

```
@misc{gupta2021clsril23,
      title={CLSRIL-23: Cross Lingual Speech Representations for Indic Languages}, 
      author={Anirudh Gupta and Harveen Singh Chadha and Priyanshi Shah and Neeraj Chimmwal and Ankur Dhuriya and Rishabh Gaur and Vivek Raghavan},
      year={2021},
      eprint={2107.07402},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

<hr>

