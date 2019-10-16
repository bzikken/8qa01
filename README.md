# Course Project: Image Analysis for cancer risk assessment (8QA01)


## Getting started 

In this project you will work with Python. This means you will need an to install software to run and edit Python code. We have a tutorial which guides you through this here: https://github.com/tueimage/essential-skills/blob/master/python-essentials.md 

For this course you can use Jupyter Notebook which is covered in the tutorial, but other software (if you use it in other subjects) is also possible. 

## Structure

The overall project steps can be found in the notebook (project_walkthrough.ipynb), which already contains a general script to go through all the images, measure simple features, and create a plot of the measurements. You can use this notebook/script for your project as well, but implement additional functions for measurement and analysis. 

The functions needed to measure features are found in the Python module utilities_8qa01.py, which currently contains two functions. This is where you should add more functions for completing your project. 

## Data

To get started with the project, we will need some images. We use images from the following paper:

Codella N, Gutman D, Celebi ME, Helba B, Marchetti MA, Dusza S, Kalloo A, Liopyris K, Mishra N, Kittler H, Halpern A. "Skin Lesion Analysis Toward Melanoma Detection: A Challenge at the 2017 International Symposium on Biomedical Imaging (ISBI), Hosted by the International Skin Imaging Collaboration (ISIC)". arXiv: 1710.05006 [cs.CV] Available: https://arxiv.org/abs/1710.05006


To get the data, go to this page https://surfdrive.surf.nl/files/index.php/s/nMApH6fK10RjSMa and download two things:  

- Large zipfile with the images
- Excel files corresponding to your group

In the zipfile you will find subfolders with two types of images:

-	ISIC_[ID].png with a lesion
-	ISIC_[ID]_segmentation.png with a mask showing which pixels belong to the lesion

The Excel files contain information about the images. One image ID corresponds to one row, and one piece of information (such as a measurement of the image) corresponds to one column. 

## Intermediate assignment

Hand-in your by-hand annotations (for your group images), following the template in group2019_example_labels.xlsx:  

- The first column ID should contain the IDs (without the file extension) of your images
- The other columns should be named FeatureName_GroupNumber_AnnotatorNumber
- The columns Melanoma etc are just examples, you do not have these yet, so you can ignore them
- The annotations in one column have to be made by one person
- The annotations have to be numeric, either integers (0,1,2..) or decimals (1.5…) are allowed
- The first sheet should not contain anything else, except the columns above
- The second sheet "key" should have short descriptions of the features 
- Call your file group2019_XY_manual.xlsx



## Code tips

When extending the code, keep in mind the following:

- Separate data and code. For example if you use a threshold value, it should be defined as a variable so it is easy to change, and not hard-coded in the function. 

- Use consistent and descriptive variable and function names (for example shape_area instead of a) 

- Comment your code, especially when it is not possible to read from the statement what is happening (for example, calculate_area(shape) is clear enough) 



## Handing in your project

For the final assignment you have to hand in your report (see the Casusinfo) and your code. You can hand in the code this with a ZIP file. Some tips:

-	Your main script has to be called group2019_XY.ipynb where XY is the group number. This script has to perform everything that is necessary to create your measurements and experiments.  

- Include the Excel file that your code creates (group2019_automatic.xlsx)

-	All necessary code (except common Python packages) needs to be included in the zip file. 

- Do NOT include the images in the zip file. 

-	The code has to run if it is unzipped on a different computer, after changing the directory where the images are located.

-	Follow the guidelines above for using comments, and separating your parameters from your code. 



