# Problem Statement
The quest for gender parity has continued to grow over the years. Gender Development Index (GDI) is one of those parameters of assessing gender equality.  GDI on the one hand is a measure of the gender gaps within key development indices. The key index of comparison is known as Human Development Index (HDI). [United Nations Development Programme (UNDP)](https://hdr.undp.org/en/content/gender-development-index-gdi?utm_source=EN&utm_medium=GSR&utm_content=US_UNDP_PaidSearch_Brand_English&utm_campaign=CENTRAL&c_src=CENTRAL&c_src2=GSR&gclid=Cj0KCQjw-JyUBhCuARIsANUqQ_KWhmZEJ4ewUgU07Ozo0CM8BEUp5cbuZEEUFzv6m1ftWN_3XceTNFgaAju6EALw_wcB) on the hand defines GDI as the ratio of female HDI to the male HDI derived from the critical areas of human development, namely: health, knowlegde and standard of living. Most countries of the world have laws and policies aimed at bridging the gaps in GDIs. GDI of 1 means that men and women development indices are equal, whereas a GDI more than one reveals that women experience better development than men. On the other hand, GOne may wonder, if GDI is synomous to gender equality. The answer is not necessarily so. However, there is a UNDP defined index for measuring gender inequality known as gender inequality index (GII). 

## Business Understanding

* Does Gender Development Index (GDI) of one mean Gender Equality?

* What are the top Countries in terms of GDIs in 2019?

* Which of the HDI Indices has the highest GDI Gap?

* 10 Countries with Worst GDIs?

## Data Understanding

The data used for the analysis in this piece of work comes from [kaggle](https://www.kaggle.com/code/ayushv322/gender-development-index-pre-processing-and-eda) and was based on 2019 data from UNDP. The original dataset has a total of **190** rows and 14 features including: 

1. HDI Rank
2. Country
3. GDI_Value
4. GDI_Group
5. HDI_Female
6. HDI_Male
7. Lif_Expec_Female - Life Expectancy of Females
8. Lif_Excep_Male   - Life Expectancy of Males
9. Excep_Yrs_Schooling_Female - Expected years of schooling 
10. Excep_Yrs_Schooling_Male - Expected years of schooling 
11. Mean_Yrs_Schooling_Female - Mean years of schooling 
12. Mean_Yrs_Schooling_Male -  Mean years of schooling 
13. GNI_PC_Female  - Gross National Income Female
14. GNI_PC_Male    - Gross National Income Male


## Data Preparation

 The following 22 countries and their data are excluded in the analysis as a result of having no GDI values for the year under review: **Liechtenstein, Andorra, Palau, Bahamas, Seychelles, Grenada, Saint Kitts and Nevis, Antigua and Barbuda, Fiji, Dominica, Samoa, Turkmenistan, Marshall Islands, Kiribati, Micronesia (Federated States of), Vanuatu, Equatorial Guinea, Solomon Islands, Papua New Guinea, Djibouti, Guinea-Bissau and Eritrea.**

 Again the first row of the dataset contained only the a constant value of 2019 which was the year the dataset was collected and includes two missing values. Hence,this row was dropped. This reduced the number of rows of data or countries whose GDIs and other paramaters to 167.

 The numerical features present in the dataset were all of string type. Cleaning led to their conversions to float data type. The GNI_PC columns contains ```commas``` and as such were removed so as to work to them as numerical values they are.



