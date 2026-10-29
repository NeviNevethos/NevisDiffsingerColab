# Recommended
[NOTE] Single speaker works the same as the legacy version
<pre>
#multi speaker (lab + wav)
your_zip.zip:
    |
    |
    lang_config.yaml
    |
    your_speaker_folder_1.lang1:
        |
        |
        data_1.wav
        data_1.lab
        .
        data_2.wav
        data_2.lab
        .
        data_3.wav
        data_3.lab
        .
        ...
    |
    your_speaker_folder_2.lang2:
        |
        |
        data_1.wav
        data_1.lab
        .
        data_2.wav
        data_2.lab
        .
        data_3.wav
        data_3.lab
        .[Uploading lang_config.yaml…]()

        ...
</pre>

[lang_config.yaml](https://github.com/MLo7Ghinsan/DiffSinger_colab_notebook_MLo7/releases/download/ref/lang_config.yaml) content:
```yaml
languages: [] # to specify language dict according to the speaker folder's extension
extra_phonemes: [AP, SP] # any extras that are in your labels, eg. vf, q, cl
merged_phoneme_groups: [] # define phonemes group that has the same sound (like-phoneme) throughout the dataset across labeling systems
```
### Example:
<pre>
diffsinger_training_data.zip:
    |
    |
    lang_config.yaml
    |
    PJS.ja:
        (data)
    |
    Opencpop.zh:
        (data)
</pre>

lang_config.yaml content:
```yaml
languages: [ja, zh]
extra_phonemes: [AP, SP]
merged_phoneme_groups:
  - [zh/i, ja/i]
  - [zh/s, ja/s]
```
___
