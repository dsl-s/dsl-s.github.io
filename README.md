# Discriminating Between Similar Languages - Speech (DSL-S 2023)

In the DSL-S 2023 shared task, participants use training and development sets from the [Mozilla Common Voice](https://commonvoice.mozilla.org) (CV) to develop a language identifier for speech. The nine languages selected for the task (Swedish, Norwegian Nynorsk, Danish, Finnish, Estonian, Moksha, Erzya, Russian, and Ukrainian) come from four different subgroups of similar languages of Indo-European or Uralic language families. The test data used in this task is the Common Voice test data for the nine languages. The participants are asked not to evaluate their systems themselves nor in any other way investigate the test data before the shared task results have been published. The total amount of unpacked speech data is around 15 gigabytes.

The 9-way classification task is divided into two separate tracks.
- **Closed track:** Only the training and development data in the Common Voice dataset are allowed in the closed track, and no other data must be used. This prohibition includes systems and models trained (in an unsupervised or supervised fashion) on any other data.
- **Open track:** The use of any openly available (i.e., available to any potential shared task participant) datasets or models, not including or being trained on the Mozilla Common Voice test set, is allowed.

Both tracks use the macro F1 score over the nine languages as the ranking measure.

## Important dates

- Training/development data and features ready
- Submission of results
- System description paper deadline
- Review results
- Final (camera-ready) papers

## Provided data and features, additional data sources

We provide i-vectors, x-vectors and MFCC features the CV clips
of training and development sets of all languages.
The features were extracted using [Kaldi](https://kaldi-asr.org/),
and are available at <link_to_be_determined>.

## Baselines

## Submission instructions

## System description papers

## Organizers
