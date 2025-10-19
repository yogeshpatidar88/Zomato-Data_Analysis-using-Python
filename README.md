# Zomato Restaurant Data Analysis Project 📊

## 🌟 Project Overview

This project involves an in-depth analysis of Zomato restaurant data to extract actionable insights on customer behavior, restaurant performance, and operational trends. The goal is to answer specific business questions related to customer preferences, spending habits, ratings, and ordering modes (online vs. offline) to inform Zomato's strategic decisions, such as targeted marketing offers.

---

## 🎯 Analysis Goals (Business Questions)

The analysis is structured around answering the following six key business questions derived from Zomato's observations and strategic needs:

1.  **Customer Preference:** What **type of restaurant** do the majority of customers order from? (e.g., Casual Dining, Cafe, etc.)
2.  **Customer Engagement:** How many **votes** has each type of restaurant received from customers? (Total vote count per restaurant type).
3.  **Quality Assessment:** What are the **ratings** that the majority of restaurants have received? (Distribution of the `rate` column).
4.  **Spending Behavior:** Given that Zomato has observed most couples order online, what is their **average spending** on each order (for two people)?
5.  **Service Performance:** Which ordering **mode (online or offline)** has received the maximum rating? (A comparison of average ratings).
6.  **Targeted Offers:** Which **type of restaurant** received more offline orders, so that Zomato can provide those customers with some good offers? (Comparison of restaurant type vs. online/offline ordering).

---

## 💾 Dataset and Data Dictionary

### Dataset
The project utilizes a dataset containing comprehensive details about various Zomato-listed restaurants. The analysis will primarily focus on key columns related to restaurant type, ratings, votes, and approximate cost.

### Key Columns for Analysis
| Column Name | Description | Role in Analysis |
| :--- | :--- | :--- |
| `listed_in(type)` | The type or category of the restaurant (e.g., Delivery, Dine-out). | Used for grouping and identifying customer preference (Q1, Q2, Q6). |
| `votes` | The total number of customer votes/reviews. | Used for calculating engagement per type (Q2). |
| `rate` | The average rating of the restaurant (e.g., 4.2). | Used for distribution analysis (Q3) and service comparison (Q5). |
| `approx_cost(for two people)` | The estimated cost for a meal for two people. | Used for calculating average spending (Q4). |
| `online_order` | Whether the restaurant accepts online orders ('Yes'/'No'). | Used for comparing service modes (Q5, Q6). |

---

## 🛠️ Technologies and Libraries

This project is built using **Python** and relies on the following popular data science libraries:

* **`pandas`**: Essential for data loading, cleaning, manipulation, and preparation (e.g., handling missing values, creating pivot tables).
* **`numpy`**: Used for numerical operations.
* **`matplotlib` (as `plt`)**: Used for generating standard statistical plots like histograms.
* **`seaborn` (as `sns`)**: Used for creating advanced and aesthetically pleasing visualizations like count plots, box plots, and heatmaps.

### Installation

You can install the required libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn
