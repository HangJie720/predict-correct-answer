# Making predictions from a DataShop dataset
<a style="margin:30px" href="https://www.featuretools.com">
    <img width=50% src="https://www.featuretools.com/wp-content/uploads/2017/12/FeatureLabs-Logo-Tangerine-800.png" alt="Featuretools" />
</a>

In this tutorial, we show how to predict whether a student will succesfully answer a problem using a dataset from [CMU DataShop](https://pslcdatashop.web.cmu.edu/). While online courses are logistically efficient, the structure can make it more difficult for a teacher to understand how students are learning in their class. To try to fill in those gaps, we can apply machine learning. However, building an accurate machine learning model requires extracting information called **features**. Finding the right features is a crucial component of both finding a satisfactory answer and of interpreting the dataset as a whole. The process of **feature engineering** is made simple by [Featuretools](http://www.featuretools.com).

*If you're running the [notebook](Demo%20-%20DataShop.ipynb) yourself, please download the [geometry dataset](https://pslcdatashop.web.cmu.edu/DatasetInfo?datasetId=76) into the `data` folder in this repository. You will only need the `.txt` file. The infrastructure in that notebook will work with **any** DataShop dataset, but you will need to change the filename to the dataset you'd like to load.*

## Highlights
* Show how to import a DataShop dataset into featuretools
* Demonstrate efficacy of automatic feature generation by training a machine learning model 
* Give an example of how Featuretools can reveal and help answer interesting questions

Here is a plot of two automatically generated features: 

![Example image](data/images/exampleimage.png)

This is an image of the average time spent on a problem versus the success rate on a given problem. There is an [interactive version](https://www.featuretools.com/wp-content/uploads/2018/03/difficulty_vs_time.html) of this plot which lets you hover over individual points to see the problem and problem step. Notice that the success rate on problems that take longer is uniformly lower for this dataset.

## Demonstration

The main notebook can be found [here](Demo%20-%20DataShop.ipynb). To run the notebook, you will need to download Featuretools with
```
pip install featuretools
```
and the geometry dataset from [the datashop website](https://pslcdatashop.web.cmu.edu/DatasetInfo?datasetId=76) (free account required). Take the `.txt` file from the zipped download and place it in the `data` folder in this repository. The notebook relies on a `datashop_to_entityset` function which is described in depth in the [entityset_function notebook](entityset_function.ipynb).

## Feature Labs
<a href="https://www.featurelabs.com/">
    <img src="http://www.featurelabs.com/wp-content/uploads/2017/12/logo.png" alt="Featuretools" />
</a>

Featuretools was created by the developers at [Feature Labs](https://www.featurelabs.com/). If building impactful data science pipelines is important to you or your business, please [get in touch](https://www.featurelabs.com/contact.html).
