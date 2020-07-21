# JASS: Japanese-specific Sequence to Sequence Pre-training for Neural Machine Translation

## Requirements
Install OpenNMT-py and subword-nmt.
```bash
pip install OpenNMT-py
pip install subword-nmt
```

## Pre-trained JASS models
We release 2 kinds of JASS models: ja+en, ja+ru. For Japanese seq2seq pretraining, we use our proposed JASS methods while MASS is utilized for English and Russian. Below are the pretrained models:
|Model|vocabulary|BPE codes|
---|---|---
|[JASS-jaen](http://lotus.kuee.kyoto-u.ac.jp/~zhuoyuanmao/jaen/model_step_80000.pt)|[ja-en](http://lotus.kuee.kyoto-u.ac.jp/~zhuoyuanmao/jaen/vocab)|[ja-en.bpe.codes](http://lotus.kuee.kyoto-u.ac.jp/~zhuoyuanmao/jaen/joint_bpe.codes)|
|[JASS-jaru](http://lotus.kuee.kyoto-u.ac.jp/~zhuoyuanmao/jaru/model_step_92500.pt)|[ja-ru](http://lotus.kuee.kyoto-u.ac.jp/~zhuoyuanmao/jaru/vocab)|[ja-ru.bpe.codes](http://lotus.kuee.kyoto-u.ac.jp/~zhuoyuanmao/jaru/joint_bpe.codes)|

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
