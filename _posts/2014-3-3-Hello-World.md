---
layout: post
title: Prediction of Wheat Crop Yield in India
published: true
---

Leveraging Data Science and Satellite Imagery

## Introduction

In a country like India, where agriculture forms the backbone of the economy, predicting crop yields accurately is not just a scientific pursuit but a necessity. With a focus on wheat – one of India's staple crops – our recent project leveraged the power of data science and satellite imagery to predict yields. This blog post delves into the intricate process of using harmonized satellite data from Sentinel, Landsat, MODIS, and ISRO's Bhuvan portal, combined with ground-level data, to create a robust multimodal model for wheat yield prediction.

![](https://raw.githubusercontent.com/milind-soni/milind-soni.github.io/master/_posts/DALL·E%202024-01-31%2018.33.10%20-%20A%20polished%20and%20professional%20digital%20illustration%20suitable%20as%20a%20header%20for%20an%20article%20about%20agricultural%20technology%20in%20India.%20The%20image%20should%20symboliz.png)



## The Challenge

Predicting agricultural yields, especially for a crop as vital as wheat, is complex. It involves understanding numerous variables - weather patterns, soil conditions, agricultural practices, and more. Traditionally, this prediction relied heavily on historical yield data and basic meteorological information. However, the advent of satellite technology and advanced data science techniques has revolutionized this field.

## Our Approach



### 1. Data Collection and Integration

**Satellite Imagery**: We utilized harmonized data from Sentinel, Landsat, and MODIS satellites. This imagery provided us with high-resolution insights into the wheat-growing regions across India, allowing us to analyze vegetation health, moisture levels, and changes over time.

![Screenshot 2024-01-31 at 6.49.22 PM.png]({{site.baseurl}}/_posts/Screenshot 2024-01-31 at 6.49.22 PM.png)


![Screenshot 2024-01-31 at 6.22.39 PM.png]({{site.baseurl}}/_posts/Screenshot 2024-01-31 at 6.22.39 PM.png)


**Soil Data**: Leveraging the ISRO Bhuvan portal, we obtained detailed soil condition data. This included soil type, texture, moisture levels, and nutrient profiles, which are crucial for understanding the potential yield of a region.

![Screenshot 2024-01-31 at 6.48.32 PM.png]({{site.baseurl}}/_posts/Screenshot 2024-01-31 at 6.48.32 PM.png)


**Government Reports**: Annual yield reports released by the government for all districts in India were parsed. This data offered a solid foundation for understanding historical yields and trends.

### 2. Data Processing

Using various data preprocessing techniques, we structured the gathered data for analysis. This involved cleaning, normalization, and segmentation to ensure the data was ready for model training.

![Screenshot 2024-01-31 at 6.22.57 PM.png]({{site.baseurl}}/_posts/Screenshot 2024-01-31 at 6.22.57 PM.png)


### 3. Multimodal Model Development

We adopted a multimodal approach, integrating various data sources to feed into our predictive models. This approach allowed us to capture the complexity and variability of factors affecting wheat yield.

### 4. Machine Learning Techniques

**XGBoost**: One of the key models used was XGBoost (eXtreme Gradient Boosting), a decision-tree-based ensemble machine learning algorithm that uses a gradient boosting framework. It's particularly effective due to its ability to handle large datasets and its flexibility in modeling various aspects of the data.
![Screenshot 2024-01-31 at 6.23.12 PM.png]({{site.baseurl}}/_posts/Screenshot 2024-01-31 at 6.23.12 PM.png)


**Segmentation Techniques**: We a customised version of the Facebook SAM segment anything model along with the YOLO V8 Image classification model to the satellite imagery to identify and categorize different land parcels and land cover.


### 5. Understanding Agriculture Cycles

A critical aspect of our project was understanding the agricultural cycles in India. By analyzing satellite data over time, we inferred key stages of wheat growth and development. This helped in aligning our predictions with the actual agricultural calendar.

![Screenshot 2024-01-31 at 6.21.10 PM.png]({{site.baseurl}}/_posts/Screenshot 2024-01-31 at 6.21.10 PM.png)


### 6. Anomaly Detection

Using historical and current data, we developed methods to identify anomalies such as unexpected weather events or disease outbreaks. This added a layer of robustness to our predictions.

### 7. Crop Spectral Signature and Identification using Phenology

To enable precise crop identification and understand the phenology or growth signature of wheat, we developed comprehensive feature vectors using multiple parameters. These feature vectors were constructed by combining various datasets:

- **Spectral Data**: Utilizing the spectral signatures captured in satellite imagery, we were able to identify specific characteristics of wheat crops, such as their reflection and absorption rates at different wavelengths.

- **Temporal Data**: By analyzing changes in the satellite data over time, we could track the phenological stages of the wheat, such as germination, growth, and harvesting periods.

- **Weather Parameters**: Incorporating weather data like temperature, precipitation, and humidity helped in understanding the environmental conditions affecting the wheat growth cycle.

- **Soil Characteristics**: Data regarding soil moisture, nutrient levels, and texture were integrated to assess the health and suitability of the soil for wheat cultivation.

These multi-dimensional feature vectors enabled us not only to identify wheat crops with high accuracy but also to monitor their growth stages and health. This data was pivotal in training our machine learning models to classify and predict wheat yields.


![Screenshot 2024-01-31 at 6.21.48 PM.png]({{site.baseurl}}/_posts/Screenshot 2024-01-31 at 6.21.48 PM.png)

## Results and Implications

The multimodal model demonstrated high accuracy in predicting wheat yields. By incorporating diverse data sources and advanced analytical techniques, we were able to provide more reliable and timely predictions than traditional methods.

These predictions can aid farmers in making informed decisions about their crops, help policymakers in planning and resource allocation, and assist in managing food security in India.

## Conclusion

The fusion of data science and satellite imagery opens new horizons in agricultural yield prediction. Our project with wheat yield in India is a testament to the power of this technology in transforming how we approach agriculture and food security. As we continue to refine our models and integrate more data, the potential for even more accurate and insightful predictions is limitless.

---
