# scivision-catalog
A package holding scivision datasets and models

## Add a new model

Add your model to the `models.json`, with the following format:

```
  "model-003":{
    "task":"segmentation",
    "model":"github.com/alan-turing-institute/cv-algortithm",
    "github_branch":"master",
    "language":"Python3",
    "data_format":"tif",
    "pretrained":"yes",
    "labels_required":"yes",
    "institution":"alan-turing-institute",
    "tags": ["dummy"]
  }
```

## Add a new dataset


Add your model to the `datasources.json`, with the following format:

```
{
  "model-000":{
    "task":["object-detection", "segmentation"],
    "model":"https://github.com/stardist/stardist",
    "github_branch":"master",
    "language":"Python3",
    "data_format":"tif",
    "pretrained":"yes",
    "labels_required":"yes",
    "institution":"epfl",
    "tags": ["2D", "3D", "optical-microscopy", "xray", "microtomography", "cell-counting", "plant-phenotyping", "climate-change-and-agriculture"]
  }
 ```
