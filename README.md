# semester-project

## Getting Started

This project depends upon Spark 3.1, Pyspark, and seaborn for processing.  While most of the project was designed to target any system capable of running pyspark, there may be some unaccounted for dependencies that were configured in Rivanna.

### Obtaining source data

Due to the dataset size, it cannot be uploaded into github.  Instead, you can manually download it from Kaggle at https://www.kaggle.com/arevel/chess-games/download.

Note that the notebooks assume the CSV from the above link is placed in the file `<gitrepo>/data/raw/chess_games.csv`.

### Order of notebook execution

Notebooks should be executed in the following order to ensure all predecessor information is present.

* Data Preparation
   * `code/dataprep/01-readfilter.ipynb`
   * `code/dataprep/02-model-data.ipynb`
* Model
   * Each experement can be run independent of each other, but must be run in the numerical sequence.
   * That is, for experement-01, you will need to run notebooks `01-*.ipynb`, then `02-*.ipynb` until you reach the end.
