# Breast Cancer Detection

![image.jpg](can3.jpg)
- Cancer Detection is a one of the most resarched topic in not only in field of Medicine but also in Instrument technology and machine learning.
- Among all types of cancer breast cancer has the maximum share.
- With increase in unhealtty lifesytle and polluting envioronment it has been more important than ever to study and diagnose.
- Despite efforts on part of various agenices many lifes are lost to the deadly cause.<br>

According to WHO there are about 1.38 million new cases and 458 000 deaths from breast cancer each year (IARC Globocan, 2008)

## Methodlogy of Data Collection

![image.jpg](fna.JPG)

- The methodlogy used to collect data is Fine-needle aspiration (FNA). FNA is a diagnostic procedure used to investigate lumps or masses. In this technique, a thin (23–25 gauge), hollow needle is inserted into the mass for sampling of cells that, after being stained, will be examined under a microscope (biopsy).
- Fine-needle aspiration biopsies are very safe minor surgical procedures. Often, a major surgical (excisional or open) biopsy can be avoided by performing a needle aspiration biopsy instead, eliminating the need for hospitalization. In 1981, the first fine-needle aspiration biopsy in the United States was done at Maimonides Medical Center.[1] Today, this procedure is widely used in the diagnosis of cancer and inflammatory conditions

## Classification Problem

![image.jpg](cp.JPG)

- In Machine learning the output of detection for any disease is considered in binary format, i.e With the given data set/input data of subject/patient will infected with the given disease or not. 
- The given data or the input data is nothing but the test results that are conducted while examining the patient.

## Data set

- The dataset consist of features which are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image.

- Dataset has been downloaded from UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

- Attribute Information <br>
-- ID number <br>
-- Diagnosis (M = malignant, B = benign)<br> 
-- A benign tumor is a tumor that does not invade its surrounding tissue or spread around the body. A malignant tumor is a tumor that may invade its surrounding tissue or spread around the body.

- Ten real-valued features are computed for each cell nucleus <br>
-- radius (mean of distances from center to points on the perimeter)<br>
-- texture (standard deviation of gray-scale values)<br>
-- perimeter<br>
-- area <br>
-- smoothness (local variation in radius lengths) <br>
-- compactness (perimeter^2 / area - 1.0)<br>
-- concavity (severity of concave portions of the contour)<br>
-- concave points (number of concave portions of the contour)<br>
-- symmetry<br>
-- fractal dimension ("coastline approximation" - 1)<br>

- The mean, standard error and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.
- All feature values are recoded with four significant digits.
- Missing attribute values: none
- Class distribution: The data here is not very much unbalanced as we see that i.e __357 benign (62.7%), 212 malignant(37.3%)__
- The data set has __569 rows and 33 columns__.

# EDA
- List of columns 
- id, diagnosis, radius_mean, texture_mean, perimeter_mean, area_mean, smoothness_mean, compactness_mean, concavity_mean,
 concave points_mean, symmetry_mean, fractal_dimension_mean, radius_se, texture_se, perimeter_se, area_se, smoothness_se,
 compactness_se, concavity_se, concave points_se, symmetry_se, fractal_dimension_se, radius_worst, texture_worst,
 perimeter_worst, area_worst, smoothness_worst, compactness_worst, concavity_worst, concave points_worst,
 symmetry_worst, fractal_dimension_worst, Unnamed: 32
- Of 33 columns, "Unnamed: 32" is one of those that has no value populated and hence will be dropped.
- The dependent variable i.e __diagnosis__ is categorical and hence will be converted to numerical.

# Classifier used
- Initially the __Random Forest Classifier__ has been used. It has taken __209 seconds__ and has presented __95%__ accuracy.
- Further to optimize the approcah, __Principal component analysis__ has been taken in to consideration. It has taken __169 seconds__ and has presented __92 %__ accuracy 




