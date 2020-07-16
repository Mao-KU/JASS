# JASS: Japanese-specific Sequence to Sequence Pre-training for Neural Machine Translation

## Pre-trained JASS models
We release 3 kinds of JASS models: ja+en, ja+ru, ja+en+ru. For Japanese seq2seq pretraining, we use our proposed JASS methods while MASS is utilized for English and Russian. Below are the pretrained models:
|Model|vocabulary|BPE codes|
---|---|---
|JASS(jaen)|||
|JASS(jaru)|||
|JASS(jaenru)|||

## Usage
Please run the bpe precrocessing for the dataset to be finetuned first. After setting up the downloaded vocabulary for src and tgt sentences during the preprocessing, use ```train_from``` in OpenNMT to implement the finetuning.  

## Reference
[1] Zhuoyuan Mao, Fabien Cromieres, Raj Dabre, Haiyue Song, Sadao Kurohashi, [*JASS: Japanese-specific Sequence to Sequence Pre-training for Neural Machine Translation*](https://www.aclweb.org/anthology/2020.lrec-1.454/)

```
@inproceedings{mao-etal-2020-jass,
    title = "{JASS}: {J}apanese-specific Sequence to Sequence Pre-training for Neural Machine Translation",
    author = "Mao, Zhuoyuan  and
      Cromieres, Fabien  and
      Dabre, Raj  and
      Song, Haiyue  and
      Kurohashi, Sadao",
    booktitle = "Proceedings of The 12th Language Resources and Evaluation Conference",
    month = may,
    year = "2020",
    address = "Marseille, France",
    publisher = "European Language Resources Association",
    url = "https://www.aclweb.org/anthology/2020.lrec-1.454",
    pages = "3683--3691",
    language = "English",
    ISBN = "979-10-95546-34-4",
}
```
