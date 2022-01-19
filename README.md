# scivision-catalog
A package holding scivision datasets and models

## Extending the catalog of models and datasets

Create a new branch and do one or both of the following, before launching a pull request for your additions to be reviewed:

## Add a new model

Add your model to the end of `models.json`, with the following format, incrementing the model number by one:

```
  "model-XXX":{
    "task":"segmentation",
    "model":"github.com/alan-turing-institute/my-model",
    "github_branch":"master",
    "language":"Python3",
    "data_format":"tif",
    "pretrained":"yes",
    "labels_required":"yes",
    "institution":"alan-turing-institute",
    "tags":[
      "help-needed", "3D", "cell", "cell-counting", "biology", "biomedical-science" 
    ]
  }
```

## Add a new dataset

Add your dataset to the end of `datasources.json`, with the following format, incrementing the data number by one:

```
  "data-XXX":{
    "task":["object-detection", "segmentation"],
    "domain":["optical-microscopy"],
    "datasource":"https://github.com/my_datasource/releases/download/0.3.0/demo.zip",
    "format":"tif",
    "labels":"yes",
    "institution":"alan-turing-institute",
    "tags":[
      "help-needed", "3D", "cell", "cell-counting", "biology", "biomedical-science" 
    ]
  }
 ```
