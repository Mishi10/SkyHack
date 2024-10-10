# skyhack
This project focuses on analyzing customer call data to identify the most common issues for the airline services, calculate AHT (Average Handle Time) and AST (Average Speed to Answer), and explore trends that may contribute to increased call durations.

## Table of Contents
1. [Introduction](#introduction)
2. [Google Colab Setup](#google-colab-setup)
3. [Usage](#usage)
4. [Dataset](#dataset)
5. [Results](#results)
6. [Solution](#solution)
7. [Contributing](#contributing)
 

## Introduction

Customer service performance is critical for ensuring customer satisfaction. This project aims to:
- Analyze key call metrics such as AHT and AST.
- Uncover common customer problems contributing to higher AHT and AST.
- Visualize the patterns and provide insights to improve customer service processes.

## Google Colab Setup

To run the analysis using Google Colab, follow these steps:

### 1. Open Google Colab

Click [here](https://colab.research.google.com/) to open Google Colab.

### 2. Clone the Repository

In your Colab notebook, clone the project repository using the following command:

```python
!git clone https://github.com/Khushitatwal/skyhack.git
```
### 3. Change the directory
Once the repository is cloned, navigate to the project directory:
```
%cd skyhack
```
### 4. import libraries 
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import re
from collections import Counter
```
## Usage
After setting up the environment, you can run the analysis using the provided Colab cells.

## Dataset
This dataset is used to analyze customer call data, focusing on key performance metrics such as **Average Handle Time (AHT)** and **Average Speed to Answer (AST)**. The dataset also contains customer transcript data, allowing us to identify common issues and trends in customer interactions.
The dataset contains information on customer service calls with various fields capturing details like call duration, reason for the call, and customer loyalty level.  
## Results
Based on dataset analysis, the most frequent reason for calls are
 - **Checkout**, **ETC**, **Post-Flight**, and **Mileage Plus** issues result in significantly longer Average Handle Times (AHT).
 - **Checkout**, **Traveler Updates**, **Unaccompanied Minor**, and **Seating** inquiries contribute to higher Average Speed to Answer (AST).
 - **IRROPS (Irregular Operations)** and **Voluntary Changes** are often left unresolved, indicating possible gaps in agent training or process inefficiencies.
 - AST spikes occur at **3 A.M., 7 A.M., and 7 P.M.**, while average AST is observed at **5 A.M., 12 P.M., 2 P.M., 5 P.M., and 9 P.M.**.
 - **Customer membership Impact on AHT and AST:**
     - **Elite-level customers** experience **faster response times (lower AST)** but typically require **longer handling times (higher AHT)** due to more complex inquiries or personalized service.
     - **New or non-elite customers** experience **longer waiting times (higher AST)** but their calls are generally shorter and less complex, leading to a **lower AHT**.

Based on the transcript analysis, the most frequent terms found in calls with high AHT and AST include words like flight, agent, customer, change, and help. These likely reflect the common issues customers encounter:

 - Flight rescheduling or changes
 - Requests for help or agent assistance
 - Customer account changes

## Solution
- Optimize the call routing system to handle complex issues faster and reduce AHT for elite customers.
- Improve agent training and knowledge-sharing on frequent unresolved issues like IRROPS and voluntary changes.
- Adjust staffing levels to address peak AST times for better resource management.
- Improve the IVR systems for the issues and information related to checkout , refund , flight change ,delay enquires.

## Contributing
If you'd like to contribute to improving the dataset or analysis, please fork the repository and submit a pull request.

 
