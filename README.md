# Discriminating Between Similar Languages - Speech (DSL-S 2023)

In the [VarDial 2023](https://sites.google.com/view/vardial-2023) DSL-S shared task, participants use training and development sets from the [Mozilla Common Voice](https://commonvoice.mozilla.org) (CV) to develop a language identifier for speech. The version to be used is Common Voice corpus 12.0 published 7.12.2022. The nine languages selected for the task (Swedish, Norwegian Nynorsk, Danish, Finnish, Estonian, Moksha, Erzya, Russian, and Ukrainian) come from four different subgroups of similar languages of Indo-European or Uralic language families. The test data used in this task is the Common Voice test data for the nine languages. The participants are asked not to evaluate their systems themselves nor in any other way investigate the test data before the shared task results have been published. The total amount of unpacked speech data is around 15 gigabytes.

For each language, only the audio files indicated in the train.tsv and dev.tsv files should be used for training. The metadata in the train.tsv and dev.tsv can be used for training purposes. The metadata includes the transcripts and they can also be used in training, but they will not be available when processing the test data.

The 9-way classification task is divided into two separate tracks.
- **Closed track:** Only the training and development data in the Common Voice dataset are allowed in the closed track, and no other data must be used. This prohibition includes systems and models trained (in an unsupervised or supervised fashion) on any other data.
- **Open track:** The use of any openly available (i.e., available to any potential shared task participant) datasets or models, not including or being trained on the Mozilla Common Voice test set, is allowed.

Both tracks use the macro F1 score over the nine languages as the ranking measure. We will also report micro F1 scores for the larger picture.

## Important dates

- Training/development data and features ready
- Submission of results
- System description paper deadline
- Review results
- Final (camera-ready) papers

## Data, baselines features, additional data sources

We provide a simple baseliene at <https://github.com/dsl-s/baselines>.

The audio data provided as MP3 files by the [Mozilla Common Voice](https://commonvoice.mozilla.org). We also provide pre-computed i-vectors, x-vectors and MFCC features extracted using [Kaldi](https://kaldi-asr.org/). The pre-computed features can be downloaded from [Zenodo](https://zenodo.org/record/7555151). The baseline repository also includes helper scripts for downloading the source data and pre-computed features.

## Submission instructions

TBA

## System description papers

TBA

## Organizers
