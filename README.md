## Example-Work
The example work repository is comprised of projects completed by myself, and classmates, during the course of my Data Analytics Engineering Coursework. 
The programs are typically completed using R and Python in R Studio and Jupyter Notebooks respectively.

## System Requirements
R Studio Download Here: https://www.rstudio.com/products/rstudio/download/
Jupyter Notebook Download Instructions:
  1) Proceed to download Anaconda Navigator, which is a desktop application allowing easy access to open-source programs for data science and other needs:
    https://www.anaconda.com/products/individual
  2) Once downloaded, open the Anaconda Navigator and Launch a Jupyter Notebook. This will open a local version of Jupyter Notebooks and then allow you to open any Jupyter
  files inside the repository (file type ending .ipynb).
  
## Random Forests Classifier Model

In our Data Analytics Engineering Summer 2021 Course, AIT 580, we were tasked with finding a problem and dataset, then attempting to create a model designed to solve this problem.
For our project, our group decided to take on a Department of Justice challenge that surrounded the recidivism of inmates and whether one could predict if an inmate would recidivate and, if possible, what year (first year, second year, or third year out of prison) they recidivate in. The dataset was provided to us and was taken from the Georgia Department of Community Supervision. The training dataset, which we used for our modeling, was comprised of over 18,000 instances with 54 columns. That dataset is provided explained and provided here: https://data.ojp.usdoj.gov/stories/s/daxx-hznc

Utilizing Python through Jupyter Notebook, we proceeded to pre-process the data by accounting for NULL/Unkown values and Label Encoding the string, categorical attributes that persisted throughout. This was necessary for Random Forests Classifier as Random Forests cannot run when there are NA values and will not be able to utilize string values in its predictions. It will not know what the string means.

Once done, we conducted exploratory data analysis in Python and Tableau. A public Tableau workbook, allowing anyone to explore the dataset, can be found here: https://public.tableau.com/app/profile/ryan6250/viz/RecidivisminGeorgia/RecidivisminGeorgia.

After exploratory data analysis, and initial test runs of the model, we decided to proceed with two models. One would be attempting to predict whether they recidivated at all, and the other would attempt to predict the specific year of recidivism, if they did recidivate.

After utilizing GridSearchCV to test a variety of hyperparameters, our most efficient model was able to predict the multi-categorical variable with 54% accuracy. Our most efficient model was able to predict the binary variable with 72.8% accuracy.

Alongside, Random Forests Classifier. XGBoost Classifier was tested and was found to produce the highest accuracy, with 75.1%. 

