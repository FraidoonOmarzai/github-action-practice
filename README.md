# github-action-practice


## Steps:

* Data set downloaded and processed, and model trained on the dataset (**Note:** we were not able to download the data using the given link but i downloaded from the actual [url](https://www.sciencedirect.com/science/article/pii/S2352340920303048))

To stop tracking from Git:
```bash
            git rm -r --cached 'data_processed.csv'
            git commit -m "stop tracking data_processed.csv"
```
* We will use dvc pipelines [link](https://dvc.org/doc/start/data-management/data-pipelines#data-pipelines)

```bash
    dvc init
```

Creating dvc.yaml file using [code](https://dvc.org/doc/command-reference/run):
```bash
    dvc run -n process -d process_data.py -o data_processed.csv --no-exec python process_data.py
```

* push the code to github

* create the .github/workflow/train.yaml and copy the code inside train.yaml  => (making CML workflow)






















```bash

```