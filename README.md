# Exploratory-Data-Analysis-I-in-R
Exploratory Data Analysis part I in R by Robby Ananta

## Introduction
In this repository, a glimpse of Exploratory Data Analysis will be shown on Ames housing dataset using set of questions provided

## Steps
- MIssing value check and handling
- Duplicated value check and handling
- Filtering dataset for unusual mistakes or extreme values

## Set of Questions and Findings
### Finding missing values
1.  How many columns that have missing values ?
    
    19 out of 81 entry columns
    
2.  How many columns that have missing values more than 60% ?

    4 missing values: PoolQC, MiscFeature, Alley, Fence

3.  "Garage" related column have the same Null pct, can you guess what Null values in Garage column mean ?

    The specific housing filtered do not own a garage

### Duplicated values
1.  How many records that are duplicates ?

    There are no duplicated records

### Mistakes and Extreme values
1.  House's ID that Have unusual Sold Year is ...

    ID 524. That have been Built and Sold in year 2007, yet undergoing RemodAdd in year 2008
    
2.  How many house, sold with unusual price?

  #### count(price_upnormal)
    
    hasilnya adalah 9 house sold

3.  in which neighborhood do the unusual house sold?

  #### price_upnormal %>%
      count(Neighborhood)
    
    hasilnya adalah NoRidge: 3 house, NridgHt: 3 house, dan StoneBr: 3 house
