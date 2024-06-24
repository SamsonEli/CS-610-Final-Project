# CS 610 Group 6 Final Project - Spoiled Meat Detection to Prevent Foodborne Illness


## Overview
Access to enough safe and nutritious food is key to sustaining life and promoting good health. Unsafe food that contains harmful bacteria, viruses, parasites, or chemicals can lead to over 200 diseases, ranging from nausea, fever and perhaps even cancer (World Health Organization, 2022). Ingestion of such bacteria typically will result in gastroenteritis, where the symptoms typically include but not limited to are nausea, fever, bloating and vomiting (Johns Hopkins Medicines, n.d.). Vulnerable groups, including young children, seniors, pregnant women, and individuals with chronic diseases, face a higher risk of fatality if food safety is not properly managed. 

An estimated of 600 million people fall ill after eating contaminated food, leading to approximately 420,000 deaths annually. (World Health Organization, 2022) As global meat consumption continues to rise steadily over the years (Statista, 2024), ensuring the safety of food becomes increasingly crucial to prevent further casualties and fatalities. A robust system needs to be implemented to track meat quality before consumption. In this research paper, we will be exploring Artificial Intelligence technology and will be utilizing Machine Learning to evaluate the effectiveness of the various models (Qing, Zhang, & Wang, 2022).

## Background Information
The predominant bacteria associated with spoilage of refrigerated beef and pork, are Brochothrix thermosphacta, Carnobacterium spp., Enterobacteriaceae, Lactobacillus spp., Leuconostoc spp., Pseudomonas spp. and Shewanella putrefaciens (Borch, Kant-Muermans, & Blixt , 1996). It is known that bacteria are a few of the microbes that can generate natural colors (Agarwal, et al., 2023). A snapshot of the listed bacteria is provided in the appendix as Figure 2.

Deep learning models can classify images by breaking them down into their RGB values and using convolutional layers to detect patterns and features at various levels of abstraction. (Nisha, Sathik, & Meeral, 2020). As a result, we will be exploring the various Machine Learning models, including self-built ones, to see which the best model is to detect whether the meat has turned stale.
 

## Performance Metrics

Given the potentially life-threatening effects of consuming spoiled meat, it is crucial to minimize false negatives, specifically cases where the model predicts ‘Spoiled’ meat as ‘Half-fresh’ or ‘Fresh’. Thus, recall for ‘Spoiled’ meat is a critical metric, measuring the proportion of correctly detected ‘Spoiled’ instances. Due to the importance of recall, the F3 score is the focus in terms of performance metrics. It is calculated using the following equation:

\[ \text{F3 Score} = \frac{(1 + \beta^2) \cdot \text{Precision} \cdot \text{Recall}}{(\beta^2 \cdot \text{Precision}) + \text{Recall}} \]

where \(\beta\) is 3, giving more weight to recall compared to precision. The F3 score is chosen as the critical metric over the F2 score due to the significant importance of not inaccurately mislabeling ‘Spoiled’ meat.


## Results

The below image shows a summary of the results of all the different types of machine learning models that we executed. In conclusion, we concur that the deep learning model has much better performance for image classification tasks, as seen in the Accuracy, F1, F2, and F3 scores in our results. Additionally, our fine-tuned VGG16 model has demonstrated exceptional performance, achieving a high F3 score and high accuracy results compared to the rest of the models.


![image](https://github.com/SamsonEli/CS-610-Final-Project/assets/52133028/b6de0212-ee64-4bf2-a40a-0d1bf7913e15)

## Conclusion and Future Works

To further expand the business case for future commercialization, we may consider adopting the following 3-pronged approach:

1. **Expand our dataset:**
   - Increase the number of images in our dataset (taken in different light settings).
   - Include more types of meat (fish, seafood, etc.).

2. **Marketing to the following potential business user groups:**
   - Supermarkets
   - Restaurants
   - Food Safety Regulators (such as Singapore NEA for audit purposes)
   - Household Members  

3. **Partner with a software company to launch an app with the following capabilities:**
   - Image Capturing System
   - Recording System (For commercial usage)
   - Report System (For commercial usage)

The team is confident that adopting these strategies will ensure broader applicability and enhance the robustness of our findings in practical settings.
