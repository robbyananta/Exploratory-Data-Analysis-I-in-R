# Exploratory-Data-Analysis-I-in-R
Exploratory Data Analysis part I in R by Robby Ananta

## Introduction
In this repository, a glimpse of Exploratory Data Analysis will be shown on Ames housing dataset using set of questions provided

## Steps
- MIssing value check
- Duplicated value check
- Filtering dataset for unusual mistakes or extreme values

## Set of Questions and Findings
### Finding missing values
1.  How many columns that have missing values ?
    
    19 out of 81 entry columns
    
2.  How many columns that have missing values more than 60% ?

    ![image](https://user-images.githubusercontent.com/95951930/155143776-10ba267a-59b1-42f3-85b2-5cd462a1006b.png)

    There are 4 missing values in column: PoolQC, MiscFeature, Alley, Fence

3.  "Garage" related column have the same Null pct, can you guess what Null values in Garage column mean ?

    The specific housing filtered do not own a garage

### Duplicated values
1.  How many records that are duplicates ?

    There are no duplicated records

### Mistakes

Here data YearBuilt, YearRemodAdd and YrSold is filtered to find the odd difference

![image](https://user-images.githubusercontent.com/95951930/155143368-5119cce9-1646-4904-bd5a-c258777826cc.png)

1.  House's ID that Have unusual Sold Year is ...

    ID 524. That have been Built and Sold in year 2007, yet undergoing RemodAdd in year 2008

### Extreme Values

In this section data section of data_house$SalePrice, based on min and max values observed, filter is used to dedicate the limit.
The limit would be set on house with value over $500,000 = unusual price housing.

![image](https://user-images.githubusercontent.com/95951930/155142410-86facfbe-cd54-4e1b-a7fc-1f877a22ac5a.png)

![image](https://user-images.githubusercontent.com/95951930/155142865-836e551d-9e2b-4fde-889f-4f0ebb7a7c12.png)
   
2.  How many house, sold with unusual price?

    There are 9 house sold with unusual prices based on filtered price

3.  in which neighborhood do the unusual house sold?

    The unusual house sold located in 3 neigborhoods which are: NoRidge (3 houses), NridgHt (3 house), and StoneBr (3 house)
