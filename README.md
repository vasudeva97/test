# Welcome to the SensingBridge Hackathon!

## Datasets

Multiple datasets are located in the `sensing-brige-hackathon/data/datasets` bucket on MinIO.

1. ***SGO***: This dataset contains 9 CSV files with the data from SGO client instance.
1. ***Patents***: This folder contains a CSV file with 500k patents related to drone technology from 2015 to 2021.
    1. ***Drones Reference Ontology***: Reference ontology for the Drones instance that includes the keywords that were used for querying the patent dataset.
1. ***Drones***: This data set can be used as an auxiliary data set, if a team would like to validate their models against a different dataset. Teams working on any of the problems statements may refer to this dataset. This folder contains 7 CSV files with data from our Drones client instance. 

The following table outlines which datasets are applicable for each problem statement.

#### Dataset Matrix

| Dataset | Problem Statement 1 | Problem Statement 2 | Problem Statement 3| Problem Statement 4 |
|:---|:---:|:---:|:---:|:---:|
| Drones<sup>&dagger;</sup>  |         |         |         |         |
| Patents                    | &check; |         |         | &check;<sup>&Dagger;</sup> |
| SGO                        |         | &check; | &check; | &check; |

<sup>&dagger;</sup> The Drones dataset is for reference and may be used for data exploration or validating models against a different use case.

<sup>&Dagger;</sup> Reference the **Restrictions** section for clairification on this dataset.

### Restrictions

#### Problem Statement 1:
When using the data in the Patents dataset the following rules must be followed:
- ***Patents Dataset***
    - `patents_0604.csv` **may** be used
    - `drones_reference_ontology.csv` is for **reference only**, and **not** to be used for model building

#### Problem Statement 4:
- ***SGO Dataset***
    - all data may be used
- ***Patents Dataset***
    - `patents_0604.csv` **may** be used
    - `drones_reference_ontology.csv` **may** be used for model building

## Reference Files
- ***Drones Use Case***: This file contains an overview slide for the Drones use case.
- ***Data Set Descriptions.xlxs***: This file contains a description of all CSV files in the SGO and Drones datasets. This file also contains definitions for every field within each of the files.
- ***Data Science Pipeline.pdf***: This file provides a visual description of the data science pipeline