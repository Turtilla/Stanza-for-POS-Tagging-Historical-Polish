# Can Stanza Be Used for POS-tagging Historical Polish?

This is a repository for the paper under the same title submitted and accepted to the Student Research Workshop at EACL 2024. Both the code and the data are based on [my MA thesis](https://github.com/Turtilla/swe-ma-thesis), with changes.

## REPOSITORY STRUCTURE:
* `code`: Contains all the code (and some of the data) for the project. Large models are not included.
  * `preproc_bert.py`: A script used for preprocessing files for BERT to remove unnecessary tokens (that describe the range of agglutinations of tokens).
  * `functions.py`: A Python file containing functions that are reused across multiple Jupyter Notebooks (also for the sake of keeping the notebooks shorter).
  * `requirements.txt`: A list of necessary libraries/modules (not complete).
  * **`*.ipynb`: Other notebooks detailing the evaluation of different taggers and lemmatizers.**
* `data`: Contains the majority of the data used in the project.
  * `results`: Contains both the entire tagger outputs for the historical data and the files with annotated errors, alongside generated visualizations.
  * `mistakes`: Contains the outputs of the Jupyter Notebooks with mistakes made by specific taggers or lemmatizers.
  * *`ud-treebanks`: Contains the UD treebanks out of which PDB is used - not included in this repository due to size.*
  * `memoirs*.conllu`: Different files containing preannotation or annotation in a CoNLL-U format. Refer to `memoirs_3k_corrected.conllu` for the fully corrected version (UPOS, XPOS, lemma), and `memoirs_10k_corrected.conllu` for a version with 10k tokens with manual UPOS annotation, but not all XPOS and lemma annotation has been reviewed in that file.
