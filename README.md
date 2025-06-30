# Data Analysis for an Online Retail UK Shop

---
The aim of this project is to gain deeper insights into customer behavior to enable the businesss to tailor strategies to boost revenue by reducing customer churn, increase customer loyalty and engagement.

## Overview

---
This Online Retail II data set contains all the transactions occurring for a UK-based and registered, non-store online retail between 01/12/2009 and 09/12/2011.The company mainly sells unique all-occasion gift-ware. Many customers of the company are wholesalers.

## Dataset Characteristics

* Multivariate.
* Sequential.
* Time-Series.
* Text and more.

* Instances: `1067371`
* Associated Tasks:
  * Classification
  * Regression
  * Clustering

* Source: [A Real Online Retail Transaction Dataset for two years](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

* Features: Invoice number (InvoiceNo), StockCode,Description, InvoiceDate,Quantity, InvoiceDate, UnitPrice, Country, CustomerID.

## EDA Visuals

---

1. Cluster 0 (Blue): `Retain`

* Rationale: This cluster represents high-value customers who purchaase regularly, though not always very recenct. The focus should be on retention efforts to maintain thier loyalty and spending levels.
* Action: Implement loyalty programs, personalized offers and regular engagements to ensure they remain active.

2.Cluster 1 (Orange): `Re-engage`

* Rationale: This group includes lower-value, infrequent buyers who have not purchased recently. The focus should be on re-engagement to bring them back into active purchasing behavior.
* Action: Use targeted marketing campains, special discounts, or reminders to encourafe them to return and purchase again.

3.Cluster 2 (Green): `Nurture`

* Rationale: This cluster represents the least active and lowest-value customers, but they have made recent purchases. Thes customers may be new or need nurturing to increase their engagment and spending.
* Action: Focus on building realtionships, providing excellent customer service and offering incentives to encourage more frequent purchases.

4.Cluster 3 (Red): `Reward`

* Rationale: This cluseter includes high-value, very frequent buyers, many of whom are still actively purchasing. They are your most loyal customers and rewarding thier loyalty is key to maintaining their engagement.
* Action: Implement a robust loyalty program, provide exclusive offers and recognize their loyalty to keep them engaged and satisfied.



![](https://github.com/itsmearafik/online_retail_data_clustering/blob/main/assets/clean_data_hist_visual_1.png)

<br>

Outlier Data points.

![](https://github.com/itsmearafik/online_retail_data_clustering/blob/main/assets/clean_data_outlier_box_plot_visual.png)


### Summary of Cluster Names

* Cluster 0 (Blue): "Retain"
* Cluster 1 (Orange): "Re-Engage"
* Cluster 2 (Green): "Nurture"
* Cluster 3 (Red): "Reward"

![](https://github.com/itsmearafik/online_retail_data_clustering/blob/main/assets/customer_data_cluster_scatter_plot_visual.png)

## Key Insights

---

* Cluster -1 (Monetary Outliers) `Pamper`: Characteristics - high spenders but not necessarily frequent buyers. Their purchases are large but infrequent.
    Potential strategy: Focus on maintaining their loyalty with personalized offers or luxury services that cater to their high spending capacity.

* Cluster -2 (Frequency Outliers) `Upsell`: characteristics - frequent buyers who spend less per purchase. These customers are consistently engaged but might benefit from upselling opportunities.
    Potential strategy: Implement loyalty programs or bundle deals to encourage higher spending per visit, given their frequent engagement.

* Cluster -3 (Monetary & Frequency Outliers) `Delight`: characteristics - the most valuable outliers, with extreme spending and frequent purchases. They are likely your top-tier customers who require special attentioin.
    Potential strategy: develop VIP programs or exclusive offers to maintain their loyalty and encourage continued engagement.

![](https://github.com/itsmearafik/online_retail_data_clustering/blob/main/assets/final_customer_segment_visual.png)

## How to Use

---

1. Clone the Repository:

<pre><code>git clone https://github.com/itsmearafik/online_retail_data_clustering.git
cd data-analyst-job-postings</code></pre>

2.Explore the Notebook
    * Jupyter notebook for data cleaning, analysis and visualisation are provided in `retail_cluster_app.ipynb` file.

3.View the Visualizations
    * All key insights and plots are available in the `assets/` directory.

## Requirements

---

* Python 3.8+
* Pandas
* SKlearn
* Matplotlib
* Seaborn
* Jupyter (optional, for running notebook)

## License

---

This project is for educational and research purposes. Please refer to the original [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/datasets)
