# Machine Learning Datasets

This repository contains various machine learning datasets that can be used for practicing on Google Colab. The purpose of this repository is to provide a centralized location for all datasets, and to make it easy to download and use them in Colab notebooks.

## Usage

To use the datasets in your Colab notebook, simply run the following command:

```
from pathlib import Path
import urllib.request

def load_data():
    csv_path = "filename"
    if not csv_path.is_file():
        Path("datasets").mkdir(parents=True, exist_ok=True)
        url = "https://github.com/Nisarg6502/ML_Datasets/remaining file path"
        urllib.request.urlretrieve(url, csv_path)
    return pd.read_csv(csv_path)

housing = load_data()
```
