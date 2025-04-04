# Big Data Parallel Programming Course (LAB 1: Installation using Conda inside Visual Studio Code)

## Pre-requesters
- This Lab is done in VS code

## Create Visual Studio Code Project Folder using file explorer or command line 

## Open Project/Folder in Visual Studio Code

## Create conda environment
Press Ctrl+Shift+P (Windows/Linux) or Cmd+Shift+P (Mac) to open the Command Palette.

In the Command Palette, type Python: Create Environment and select it.

**If don't have conda, install it using** https://www.anaconda.com/docs/getting-started/miniconda/main

![](Create_Env_1.png)

Select conda environment
![](Create_Env_2.png)

Select Python 3.8
![](Create_Env_3.png)

You should see something similar at the bottom right corner
![](Create_Env_4.png)
![Conda_Install_Success.png](Conda_Install_Success.png)

## Open Visual Studio Code Terminal and check currently activated conda environment
![Open_Terminal.png](Open_Terminal.png)

![](Check_Env_2.png)

`conda env list` will list available environments and highlight (*) the current activated one

![](Check_Env_3.png)

## Install Apache Spark
### Check Java version inside the conda environment
``java -version``

If Java is not installed in your system you may get a similar error like this:
![Java_Not_Found.png](Java_Not_Found.png)
#### If 8 > JDK > 17, Install JDK 17
``conda install -c conda-forge openjdk=17``
#### Check Java version inside the conda environment again
``java -version``

![Java_Install_Success.png](Java_Install_Success.png)
### Install pyspark pandas and pyarrow
``pip install pyspark pandas pyarrow notebook``

## ATTENTION: command to delete conda environment (ONLY IF YOU HAVE MADE A MISTAKE)
``conda env remove --name <env name>``

## Run Lab1 notebook and submit it via Black Board

- Download [Lab1_NameSurname.ipynb](Lab1_NameSurname.ipynb).
- Run the notebook. 
- Save the notebook
- Submit the run notebook through Black Board.

# References
## Conda 
- https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html
- https://www.anaconda.com/docs/getting-started/miniconda/main

## PySpark
- Overview https://spark.apache.org/docs/latest/api/python/index.html
- Installation https://spark.apache.org/docs/latest/api/python/getting_started/install.html
