# Customer Segmentation with RFM Analysis

This project uses real-world retail transaction data to perform customer segmentation with **RFM (Recency, Frequency, Monetary)** analysis. It demonstrates the full pipeline from raw data to clustering and visualization — a key part of customer analytics and marketing data science.

---

## Files Included

- `Online_Retail_Project.ipynb` – Full annotated Jupyter notebook with data cleaning, EDA, RFM feature engineering, clustering, and visualization.
- `Online_Retail.xlsx` – Original dataset of transactions from a UK-based online retailer.
- `Customer Segment Distribution Pie Chart.png` – Pie chart visualization of customer segments by percentage.

---

## Project Goals

- Clean and prepare the dataset for analysis  
- Engineer features using the **RFM model**  
- Apply **KMeans clustering** to group customers into distinct segments  
- Visualize the clusters and segment composition using **matplotlib**  
- Assign each customer to a labeled segment (e.g. "Loyal/VIP", "Lost", etc.)

---

## Key Steps

1. **Data Cleaning**
   - Removed cancelled transactions and rows with missing customer IDs
   - Filtered out zero or negative unit prices

2. **Feature Engineering**
   - Created `TotalPrice` as `Quantity × UnitPrice`
   - Built the RFM table for each customer
   - Standardized features for clustering

3. **Clustering**
   - Used the Elbow Method to choose optimal number of clusters
   - Applied `KMeans` clustering on RFM features

4. **Segment Labeling**
   - Interpreted cluster profiles based on R, F, M scores
   - Assigned meaningful names like:
     - Loyal/VIP Customers
     - Needs Attention
     - Lost Customers
     - Recent Customers

5. **Visualization**
   - Pie and bar charts to display segment distributions

---

## Skills Demonstrated

- Data cleaning and preparation with **Pandas**  
- RFM feature engineering  
- Unsupervised learning with **KMeans**  
- Data visualization with **Matplotlib**  
- Exploratory data analysis and clustering interpretation

---

## Dataset

The data comes from the **UCI Machine Learning Repository**, originally sourced from a UK-based online retailer. It includes 500,000+ transactions between 2010 and 2011.

---

## How to Run

1. Clone this repo
2. Open `Online_Retail_Project.ipynb` in Jupyter or VS Code
3. Install dependencies:

   ```bash
   pip install pandas matplotlib scikit-learn
   ```

---

## Author

Tyler Parnell (Tp-oi), Mathematics and Big Data Student.
Feel free to reach out if you have questions about the project.

*This project was completed as part of my ongoing effort to develop my data science skills and build my portfolio.*

---

## License

This project is distributed freely under the MIT license


