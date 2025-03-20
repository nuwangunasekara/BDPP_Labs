# BigDataCourse
## Pre-requesters 
Conda 
https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html
https://www.anaconda.com/docs/getting-started/miniconda/main

## Overview
Reference https://spark.apache.org/docs/latest/api/python/index.html
## PySpark Installation
Reference: https://spark.apache.org/docs/latest/api/python/getting_started/install.html
### create cond environment and install Apache Spark
#### Create conda environment
```conda create -n pyspark_env python=3.8 pip```
#### Activate conda environment
```conda activate pyspark_env```
#### Check Java version inside the conda environment
``java -version``
##### If 8 > JDK > 17, Install JDK 17
``conda install -c conda-forge openjdk=17``
##### Check Java version inside the conda environment again
``java -version``
#### Install pyspark pandas and pyarrow
``pip install pyspark pandas pyarrow``
### delete conda environment (ONLY IF YOU HAVE MADE A MISTAKE)
``conda env remove --name pyspark_env``

## select conda env in VS Code

Press Ctrl+Shift+P (Windows/Linux) or Cmd+Shift+P (Mac) to open the Command Palette.

In the Command Palette, type Python: Select Interpreter and select it.

# Run quick starter
Download [quickstart_df.ipynb](quickstart_df.ipynb) and try running it.