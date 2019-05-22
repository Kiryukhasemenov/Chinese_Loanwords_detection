# Studies on Russian Loanword Adaptation in Chinese
### (c) Kirill Semenov, Higher School of Economics - Moscow, 2019
---
This is a coursework of Kirill Semenov, 3rd year bachelor in Computational Linguistics, HSE-Moscow.

Here you can find my dataset created on Wikidata, as well as an analysis of the Chinese Loanword Dictionary data (汉语外来词词典).

The majority of the code files are in .ipynb format, so the description of the aims and functions can be found inside (in Markdown format).

The `tranlsiterator.py` file is in .py format, so the information of the functions is in docstrings inside.

## File Description
| Type        | Filename           | Description  |
| ------------- |:-------------:| -----:|
| data (directory, .tsv files)     | [wikidata_source](../../tree/master/wikidata_source) | Tables in .tsv format, which are downloaded from Wikidata |
| data (.csv)      | [data_preprocessed_with_duplicates.csv](../../blob/master/data_preprocessed_with_duplicates.csv)      | All data from Wikidata, cleared from noise |
| data (.csv) | [data_with_duplicates_pre_final.csv](../../blob/master/data_with_duplicates_pre_final.csv)      |    All data from Wikidata, cleared from noise (supporting data, necessary for aggregation purposes) |
| data (.csv) | [data_total.csv](../../blob/master/data_total.csv)      | Main dataset for the statistic analysis |
| data (.csv) | [data_with_translit.csv](../../blob/master/data_with_translit.csv)      | Subset of Wikidata dataset with transcriptions |
| data (.csv) | [wlc_cd.csv](../../blob/master/wlc_cd.csv)      | Dataset from the Chinese Loanword Dictionary  |
| code (.py) | [transliterator.py](../../blob/master/transliterator.py)      | Algorithm for generation of Xinhua-based transliterations |
| code (.py) | [data_cleaner.ipynb](../../blob/master/data_cleaner.ipynb)      | Cleaning the Wikidata raw data (input: `wikidata_source`, output: `data_preprocessed_with_duplicates.csv`) |
| code (.py) | [dataset_aggregation.ipynb](../../blob/master/dataset_aggregation.ipynb)      | Adding Xinhua transliteration and metrics to the clean data (input: `data_preprocessed_with_duplicates.csv`, output: `data_total.csv`) |
| code (.py) | [dataset_study.ipynb](../../blob/master/dataset_study.ipynb)      | Study of the dataset, many plots inside (input: `data_total.csv`)|
| code (.py) | [bkrs_processing.ipynb](../../blob/master/bkrs_processing.ipynb)      | Creating the subset of proper names with pinyin transcriptions (input: `data_total.csv`, output: `data_with_translit.csv`)|
| code (.py) | [BKRS_study.ipynb](../../blob/master/BKRS_study.ipynb)      | Study of the phonetic adaptation of the Russian consonants (input: `data_with_translit.csv`, `wlc_cd.csv`)|
| code (.py) | [Wailaici_Cidian_comparison.ipynb](../../blob/master/Wailaici_Cidian_comparison.ipynb)      | Comparison of Xinhua prescriptions to data from Chinese Loanword Dictionary (input: , `wlc_cd.csv`)|
| document (.pptx) | [eReL_presentation.pptx](../../blob/master/eReL_presentation.pptx)      | Project presentation on "E-dictionaries and E-lexicography" conference, Zagreb, 11.05.2019|

### feel free to contact me at kir.semenow[at]yandex.ru !





