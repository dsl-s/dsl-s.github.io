# Discriminating Between Similar Languages - Speech (DSL-S 2023)

In the [VarDial 2023](https://sites.google.com/view/vardial-2023) DSL-S shared task, participants use training and development sets from the [Mozilla Common Voice](https://commonvoice.mozilla.org) (CV) to develop a language identifier for speech. The version to be used is Common Voice corpus 12.0 published 7.12.2022. The nine languages selected for the task (Swedish, Norwegian Nynorsk, Danish, Finnish, Estonian, Moksha, Erzya, Russian, and Ukrainian) come from four different subgroups of similar languages of Indo-European or Uralic language families. The test data used in this task is the Common Voice test data for the nine languages. The participants are asked not to evaluate their systems themselves nor in any other way investigate the test data before the shared task results have been published. The total amount of unpacked speech data is around 15 gigabytes.

For each language, only the audio files indicated in the train.tsv and dev.tsv files should be used for training. The metadata in the train.tsv and dev.tsv can be used for training purposes. The metadata includes the transcripts and they can also be used in training, but they will not be available when processing the test data.

The 9-way classification task is divided into two separate tracks.
- **Closed track:** Only the training and development data in the Common Voice dataset are allowed in the closed track, and no other data must be used. This prohibition includes systems and models trained (in an unsupervised or supervised fashion) on any other data.
- **Open track:** The use of any openly available (i.e., available to any potential shared task participant) datasets or models, not including or being trained on the Mozilla Common Voice test set, is allowed.

Both tracks use the macro F1 score over the nine languages as the ranking measure. We will also report micro F1 scores for the larger picture.

For general organizational information, including deadlines and system description papers, please visit main [VarDial shared tasks site](https://sites.google.com/view/vardial-2023/shared-tasks).

## Data, baselines features, additional data sources

We provide a simple baseliene at <https://github.com/dsl-s/baselines>.

The audio data provided as MP3 files by the [Mozilla Common Voice](https://commonvoice.mozilla.org). We also provide pre-computed i-vectors, x-vectors and MFCC features extracted using [Kaldi](https://kaldi-asr.org/). The pre-computed features can be downloaded from [Zenodo](https://doi.org/10.5281/zenodo.7555150). The baseline repository also includes helper scripts for downloading the source data and pre-computed features.

## Submission instructions

[The test set](https://github.com/dsl-s/baselines/raw/main/data/testset-dsl-s.tar.gz) contains only the audio files in MP3 format.
Each participant is allowed to submit 3 runs for the CLOSED submission and 3 runs for the OPEN submission to:
`ccoltekin@sfs.uni-tuebingen.de`.
Your submission files must follow the following naming convention: `DSLS-[submission_type]-run-X-[team_name].tsv`
                                                                                                                                                                                                                    
The submission files should be a tab separated file with name of the audio file
and the language id as in:
```
001.mp3	da
002.mp3 et 
003.mp3 ru
004.mp3 nn-NO
005.mp3 fi
006.mp3 myv
007.mp3 uk
008.mp3 mdf
009.mp3 sv-SE
...
```
Each submission (run) must be accompanied by a DSLTL-readme-[task_type]-run-X-[team_name].txt file containing a one-paragraph description of the respective submission, where X is the run number (1, 2 or 3).
