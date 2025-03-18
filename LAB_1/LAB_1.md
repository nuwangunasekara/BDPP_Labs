# BigDataCourse
## Pre-requesters 
Conda 
https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html
https://www.anaconda.com/docs/getting-started/miniconda/main

## Overview
Reference https://spark.apache.org/docs/latest/api/python/index.html
## PySpark Installation
Reference: https://spark.apache.org/docs/latest/api/python/getting_started/install.html
### create cond environment and install
```conda create -n pyspark_env python=3.8```

```conda activate pyspark_env```

```conda install -c conda-forge pyspark notebook pandas pyarrow```

### Use environment.yml 
```conda env create -f environment.yml``

## select conda env in VS Code

Press Ctrl+Shift+P (Windows/Linux) or Cmd+Shift+P (Mac) to open the Command Palette.

In the Command Palette, type Python: Select Interpreter and select it.

# Run quick starter
Download [quickstart_df.ipynb](quickstart_df.ipynb) and try running it.