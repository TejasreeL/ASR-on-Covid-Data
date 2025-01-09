# Association Rule Mining on COVID-19 DMO Twitter Engagement Data

## Overview  
This project focuses on discovering patterns and relationships in **COVID-19 Destination Market Organizations (DMOs) Twitter posts** and their user engagements using the **Apriori algorithm**. The goal of this project is to preprocess data effectively, extract frequent itemsets, and generate association rules with insights that can inform decisions.

Dataset link: [DMO Social Media Engagement Dataset](https://www.kaggle.com/datasets/jocelyndumlao/dmo-social-media-engagement-dataset)

## Introduction  
A DMO promotes a specific location to attract visitors and boost tourism. DMOs focus on showcasing a destination's attractions, services, and experiences through marketing campaigns, partnerships, and events. Their aim is to increase tourism and contribute to the local economy by raising awareness of the destination.

This project employs **Association Rule Mining** to analyze features from the dataset. The dataset includes both continuous and categorical variables, which are preprocessed using binning and encoding techniques. The **Apriori algorithm** is then applied to uncover frequent patterns and rules.  

## Steps  
#### 1: Importing Necessary Libraries
`Pandas`, `NumPy`, and `mlxtend` for data manipulation and ARM implementation

#### 2: Loading the Dataset  
The dataset is loaded into a Pandas DataFrame for processing.  

#### 3: Binning Continuous Data  
Continuous features such as **sentiment scores** and **user engagement metrics** are converted into five discrete categories using `binning`.  

#### 4: Encoding Categorical Data  
Categorical variables like **State** and **ContentType** are one-hot encoded using `pd.get_dummies`.  

#### 5: Combining Encoded Data with Binned Data  
The processed categorical and continuous data are merged.  

#### 6: Applying the Apriori Algorithm  
Frequent itemsets are mined with a specified **minimum support** threshold. Association rules are generated using the **confidence** metric.  

#### 7: Analyzing Results  
Rules are analyzed using metrics like support, confidence and lift, highlighting relationships between features such as sentiment, user engagement, and categorical metadata.  

## Technologies Used  
- Python  
- Pandas  
- NumPy  
- mlxtend  
