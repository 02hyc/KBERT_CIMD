# KBERT-based Chinese Idiom Misuse Detection

Run the following command:

```shell
CUDA_VISIBLE_DEVICES='0' nohup python3 -u run_kbert_cls.py \
    --pretrained_model_path ./models/google_model.bin \
    --config_path ./models/google_config.json \
    --vocab_path ./models/google_vocab.txt \
    --train_path ./datasets/idiom_sentence/train.tsv \
    --dev_path ./datasets/idiom_sentence/dev.tsv \
    --test_path ./datasets/idiom_sentence/test.tsv \
    --epochs_num 5 --batch_size 32 --kg_name HowNet \
    --output_model_path ./outputs/kbert_idiomSentence_IdiomExplanation.bin
    > ./outputs/kbert_bookreview_CnDbpedia.log &
```



